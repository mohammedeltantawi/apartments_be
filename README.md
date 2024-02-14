# Getting Started

First install using 

```
npm i
```

Then build the project using
```
npm run build
```

Finally run the server using
```
npm run start
```
The server will start running on http://localhost:9000

The server consists of three enpoints as follows

1. /apartments-list  METHOD: 'GET'
   this will return all the apartments
2. /apartments-list/add-apartment  METHOD: 'POST'
   this takes a json body with the following model
   {
     name: String,
     area: String,
     price: Number,
     resale: Boolean,
     about: String,
     bedrooms: Number,
     bathrooms: Number
   }
3. /apartments-list/apartment/:id  METHOD: 'GET'
   where the id is a query param with the id of the needed apartment
