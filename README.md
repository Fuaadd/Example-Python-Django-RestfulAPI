# Contoh RestAPI Python Django dengan sqlite
Untuk menjalankan proses backend untuk menjalankan perintah **Create (Post), Read (Get), Update (Put) dan Delete (Delete)** 

## Gunakan Postman
   ###
      1.Create data
        Response Method: POST
        Request URL: http://127.0.0.1:8000/drinks/
        form data : -data 1
                    name           lemon Juice
                    description    very fresh 
                    -data 2  
                    name           orange juice
                    description    very orange
                    
      2.cek data
        Response Method: GET
        Request URL: http://127.0.0.1:8000/drinks
        balikan : {
                  "drinks": [
                          {
                           "id": 1,
                          "name": "lemon Juice",
                           "description": "very fresh"
                           },
                           {
                           "id": 2,
                          "name": "orange juice",
                           "description": "very orange"
                           }
                           ]
                           
        Response Method: GET (cek data by id)
        Request URL: http://127.0.0.1:8000/drinks/1
        balikan : {
                  "drinks": [
                          {
                           "id": 1,
                          "name": "lemon Juice",
                           "description": "very fresh"
                           }
                           ]
                   }        
      3.Update data
        Response Method: PUT
        Request URL: http://127.0.0.1:8000/drinks/1
        pilih raw dan pilih json
        isi raw :
                  {
                  "name": "hot chocolate",
                   "description": "very hot"
                  }
        4.Hapus data
        Response Method: DELETE
        Request URL: http://127.0.0.1:8000/drinks/2
