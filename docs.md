**API Brief services and ports**
----
  <Use this API to get logs and fill the differents informations asked>

* **http://217.182.68.227:4242/**


### Endpoint /login

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
