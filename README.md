# IVoice API Documentation
Documentation for a project

## Speeches (v1/speech)
### 1. /find/{search_word}

### 2. /addnew
  To add new Speech
#### Body
```json
[
  {
      "SpeechTitle" : "Title",
      "SpeechSubject" : [ "sub1","sub2","sub3","sub4" ],
      "SpeechOrator" : [ "Orat1","Orat2","Orat3","Orat4" ],
      "SpeechUrlId" : [ 23, 24, 25 ],
      "SpeechTag" : [ "Tag1", "Tag2", "Tag3" ],
      "SpeechPublished" : 1,
      "SpeechFeatured" : 0
  }
]
```
### 3. /update/{id}
  Edit the Speech
```json
[
  {
      "SpeechID" : 3245,
      "SpeechTitle" : "Title",
      "SpeechSubject" : [ "sub1","sub2","sub3","sub4" ],
      "SpeechOrator" : [ "Orat1","Orat2","Orat3","Orat4" ],
      "SpeechUrlId" : [ 23, 24, 25 ],
      "SpeechTag" : [ "Tag1", "Tag2", "Tag3" ],
      "SpeechPublished" : 1,
      "SpeechFeatured" : 0
  }
]
```
### 4. /delete/{id}
  To delete the entire Speech
    ```json
[
  {
      "SpeechID" : 3245,
      "SpeechDeleted" : 1
  }
]
```

  
