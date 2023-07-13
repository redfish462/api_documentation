**API Brief services and ports**
----

* **http://217.182.68.227:4242/**


### Endpoint /login/

* **Method:**
 

  `POST`
  
*  **URL Params**

   **Required:**
 
   `login=[string]`

* **Data Params**

  * 

* **Success Response:**

  * **Code:** 200 <br />
    **Token:** `{token}`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Bad login" }`

### Endpoint /logs

* **Method:**
 

  `GET`
  
*  **URL Params**

  * 
   

* **Data Params**

  **Required:**
 
   `token=[string]`

* **Success Response:**

  * **Code:** 200 <br />
    **Token:** `[{log1],[log2],[log3]]`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"Bad token"`

### Endpoint /log/<id_log>/

* **Method:**
 

  `GET`
  
*  **URL Params**

  * 
   

* **Data Params**

  **Required:**
 
   `token=[string]`

* **Success Response:**

  * **Code:** 200 <br />
    **Log:** `{log}`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"Bad token"`

### Endpoint /fill/

* **Method:**
 

  `POST`
  
*  **URL Params**

  * 
   

* **Data Params**

  **Required:**
 
   `token=[string]`
   `log_id=[string]`
   `service=[string]`

* **Success Response:**

  * **Code:** 200, 400 <br />
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"Bad token|Bad log ID"`

### Endpoint /autolog/

* **Method:**
 

  `GET`
  
*  **URL Params**

  * 
   

* **Data Params**

  **Required:**
 
   `token=[string]`

* **Success Response:**

  * **Code:** 200 <br />
    **Log_id:** `{log_id}`
    **Log:** `{log}`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"Bad token|Bad log ID"`

--------------------------
    
* **Method:**
 

  `POST`
  
*  **URL Params**

  * 
   

* **Data Params**

  **Required:**
 
   `token=[string]`
   `log_id=[int]`
   `service_name=[string]`

* **Success Response:**

  * **Code:** 201 <br />
    **GOOD**
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"Bad token|Bad log ID"`
    
  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `"TRY AGAIN|BAD"`



