# Workflow Pseudocode

## 1.ProjectOverview API

### 1.1 Lambda Function to get an existing ProjectOverview

- Method: GET
- API End Point: `/Projectoverview/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Projectoverview)`
        
    1. when the user hits the`/Projectoverview/{id}:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'Projects' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
## 2. Projects API

### 2.1  Function to get all Projects

- Method: GET
- API End Point: `/Projects:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Projects)`

    1. when the user hits the`/Projects:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch All records from 'Projects' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 2.2 Function to get an existing Projects

- Method: GET
- API End Point: `/Projects/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Project)`

    1. when the user hits the`/Projects/{id}:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'Projects' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 2.3 Function to get an existing resource

- Method: GET
- API End Point: `/Projects/{id}/{resource}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(resource)`

    1. when the user hits the`/Projects/{id}/{resource}:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'resource' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

## 3. UseCases API

### 3.1  Function to get all getUseCases

- Method: GET
- API End Point: `/Usecases:`
- Request: async `(req, res)`
- Response: `res.status(200).json(/Usecases:)`

    1. when the user hits the`/Usecases:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch All records from 'Usecases' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 3.1 Function to get all getResources

- Method: GET
- API End Point: `/resource:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getResources)`

    1. when the user hits the`/resource:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch All records from 'resource' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 3.2 Function to get an existing resource

- Method: GET
- API End Point: `/resource/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getResource)`

    1. when the user hits the`/resource/{id}:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'resource' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

## Task API

### 4.1 Function to get all Task

- Method: GET
- API End Point: `/task:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getTaskList)`

    1. when the user hits the`/task:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch All records from 'task' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 4.2 Function to get an existing Task

- Method: GET
- API End Point: `/task/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getTask)`

    1. when the user hits the`/task/{id}:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'Task' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

## 5 ProjectStatus API

### 5.1 Function to get all ProjectStatus

- Method: GET
- API End Point: `/ProjectStatus:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getProjectStatus)`

    1. when the user hits the`/ProjectStatus:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch All records from 'Projects' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }

### 5.2 4.2 Function to get an existing ProjectStatus

- Method: GET
- API End Point: `/ProjectStatus/{id}/usecases:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getProjectStatusUsecases)`

    1. when the user hits the`/ProjectStatus/{id}/usecases:` endpoint an event is started.
    
    2. Import necessary modules
        - Import Client module from 'pg'

    3. Initialize PostgreSQL client
        - Initialize a new PostgreSQL client with connection details
    
    4. Connect to the PostgreSQL database
        - Connect to the database using the initialized client
    
    5. Lambda execute SQL query to fetch records by id from 'usecases' table

    6. this event triggers the corresponding lambda with the request.
    
    7. Return the successfully response object with status code 200
        - Return { statusCode: 200, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }
    
    8. Return the error response object for error status code 400
        - Return { statusCode: 400, headers: { "Access-Control-Allow-Origin": "*" }, body: JSON.stringify(objReturn) }