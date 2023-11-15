# Workflow Pseudocode
 
## 1.ProjectOverview API

### 1.1 Function to get an existing ProjectOverview

- Method: GET
- API End Point: `/Projectoverview/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Projectoverview)`
 
    1. when the user hits the`/Projectoverview/{id}:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud operation;

## 2. Projects API

### 2.1  Function to get all Projects

- Method: GET
- API End Point: `/Projects:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Projects)`

    1. when the user hits the `/projects:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 2.2 Function to get an existing Projects

- Method: GET
- API End Point: `/Projects/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(Project)`

    1. when the user hits the `/Projects:` endpoint an event is started.
    2. this event triggers the correponding lambda with request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 2.3 Function to get an existing resource

- Method: GET
- API End Point: `/Projects/{id}/{resource}:`
- Request: async `(req, res)`
- Response: `res.status(200).json(resource)`

    1. when the user hits the `/Projects/{id}/{resource}:` endpoint an event is started.
    2. this event triggers the correponding lambda with request.
    3. lambda communicates with the postgresql database and performs the related crud 
    operation;

## 3. UseCases API

### 3.1  Function to get all getUseCases

- Method: GET
- API End Point: `/Usecases:`
- Request: async `(req, res)`
- Response: `res.status(200).json(/Usecases:)`

    1. when the user hits the `/Usecases:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 3.1 Function to get all getResources

- Method: GET
- API End Point: `/resource:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getResources)`

    1. when the user hits the `/resource:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 3.2 Function to get an existing resource

- Method: GET
- API End Point: `/resource/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getResource)`

    1. when the user hits the `/resource/{id}:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

## Task API

### 4.1 Function to get all Task

- Method: GET
- API End Point: `/task:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getTaskList)`

    1. when the user hits the `/task:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 4.2 Function to get an existing Task

- Method: GET
- API End Point: `/task/{id}:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getTask)`

    1. when the user hits the `/task/{id}:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

## 5 ProjectStatus API

### 5.1 Function to get all ProjectStatus

- Method: GET
- API End Point: `/ProjectStatus:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getProjectStatus)`

    1. when the user hits the `/ProjectStatus:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;

### 5.2 4.2 Function to get an existing ProjectStatus

- Method: GET
- API End Point: `/ProjectStatus/{id}/usecases:`
- Request: async `(req, res)`
- Response: `res.status(200).json (getProjectStatusUsecases)`

    1. when the user hits the `/ProjectStatus/{id}/usecases:` endpoint an event is started.
    2. this event triggers the correponding lambda with the request.
    3. lambda communicates with the postgresql database and performs the related crud
    operation;