### Modular Monolith

### Monolith Va Microservice

### Monolith.

1. One deployment Artifact
2. Communication via method calls
3. Vertically scalable
4. One database
5. Transactions

### Microservice

1. Many deployment artifacts
2. Communication via network calls
3. Horizontally and vertically scalable
4. Many database.
5. Eventual consistency

### Modular Monolith.

Its combination of best of both worlds.

1. Physical architecture of monolith.
2. Logical architecture of microservice.
3. Ability to move microservice move easily

### Challenges in Modular Monolith

1. Defining modules and bounded context
2. Communication between modules
3. Module data independence and isolation.

### Modular Architecture for Monolith.

1. Layer architecture
2. Clean architecture
3. Vertical slice architecture.

### Communication between modules.

1. Public API -
   1. Only public API will be called to communicate between modules.
   2. Need to expose public interfaces
2. Method calls.
   1. In memory calls to access data or service.
   2. Run time coupling issues, difficult split in to an independent service in future.
3. Messaging.
   1. Asynchronous communication
   2. Only Eventual consistency.

### Module data independence

1. Every module is responsible for own data.
2. Querying data from other module directly is not allowed
3. Data Isolation.
   1. Same DB different schema or entity
      1. Don't impose foreign key constraint so that easy to migrate
   2. Different Database
   3. Different database and of type different

### Lessons learned

1. Defining module boundary.
   1. Clear separations of a logics.
   2. Spend time in understanding the module and their logic separations.
   3. Identify entities and service which can be bound together
2. Eventual consistency
3. Consider merging chatty service
4. Carefully plan to share data between module.
   1. Messaging - Most decouples solutions
   2. Module must publish message
