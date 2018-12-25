# IVoice API Documentation
Documentation for this whole project.

## I Speeches (v1/speech)
End-Point for Speeches

### 1. /find/{search_word} (GET)
Recieve a `search_word` to search the database

### 2. /addnew (POST)
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
### 3. /update/{id} (PUT)
  Edit the Speech
#### Body  
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
### 4. /delete/{id} (DELETE)
  To delete the entire Speech
#### Body  
```json
[
  {
      "SpeechID" : 3245,
      "SpeechDeleted" : 1
  }
]
```


## II Orators (v1/orator)
Next End-Point for Orators
### 1. /listall (GET)
List all the Orators
#### Body  
```json
[
  {
         "OratorName" : "Orator 1",
         "OratorHit" : 45,
         "OratorPublished" : 1,
         "OratorDeleted" : 0,
         "OratorDateAdded" : "2018-01-01T08:19:49.473",
         "OratorDateModified" :  "2018-01-10T08:19:49.473"
   }      
]
```
### 2. /add (POST)
Add new Orator 
#### Body  
```json
[
  {
         "OratorName" : "Orator 1",
         "OratorPublished" : 0,
         "OratorDeleted" : 0,
         "OratorDateAdded" : "2018-01-01T08:19:49.473",
         "OratorDateModified" :  "2018-01-10T08:19:49.473"
   }      
]
```
### 3. /edit/{id} (PUT)
To publish or Unpublish
#### Body  
```json
[
  {      "OratorId" : 6547,
         "OratorName" : "Orator 1",
         "OratorPublished" : 1,
         "OratorDeleted" : 0,
         "OratorDateModified" :  "2018-01-10T08:19:49.473"
   }      
]
```

### 4. /delete/{id} (DELETE)
To delete an orator
#### Body  
```json
[
  {      
         "OratorDeleted" : 0
   }      
]
```



## III Subject (v1/subject)
End-Point for subjects
### 1. /listall (GET)
#### Body  
```json
[
  { 
        "SubjectParent" : "Parent Subject",
        "SubjectName" : "Subject One",
        "SubjectHit" : 55,
        "SubjectPublished" : 1,
        "SubjectDeleted" : 0,
        "SubjectDateAdded" :"2018-01-10T08:19:49.473",
        "SubjectDateModified" : "2018-01-10T08:19:49.473"
  }      
]
```

### 2. /add (POST)
Add new subject
#### Body  
```json
[
  { 
        "SubjectParent" : "Parent Subject",
        "SubjectName" : "Subject One",
        "SubjectPublished" : 1,
        "SubjectDateAdded" :"2018-01-10T08:19:49.473",
        "SubjectDateModified" : "2018-01-10T08:19:49.473"
  }      
]
```

### 3. /edit/{id} (PUT)
Edit a Subject
#### Body  
```json
[
  { 
        "SubjectParent" : "Parent Subject",
        "SubjectName" : "Subject One",
        "SubjectPublished" : 1,
        "SubjectDateModified" : "2018-01-10T08:19:49.473"
  }      
]
```


### 4. delete/{id} (DELETE)
Delete a subject
#### Body  
```json
[
  { 
        "SubjectId" : 4866,
        "SubjectDeleted" : 0,
        "SubjectDateModified" : "2018-01-10T08:19:49.473"
  }      
]
```

  
