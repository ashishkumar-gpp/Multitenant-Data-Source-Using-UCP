# Single-Multitenant-Data-Source-Using Oracle UCP

Prerequisite .

**DB changes :** 
  1. You must have one CDB 
  2. create two PDBs PDB1 and PDB2 in your CDB.
  3. Create new user test_user1 in PDB1 and import DB in this schemas
  4. Create new user test_user2 in PDB2 and import DB in this schemas
  
  **Jars**
  1. add UCP Jar (ucp-21.9.0.0.jar) in your classpath
  2. Add relevent hibernate5 Jars in your class path 

**Java Code**
1. Add properies in hibernate.cfg.xml and persistence.xml file as shown in sample code.
2. MapMultiTenantConnectionProvider.getSharedUCPCOneectionPDB (...) could be used in your custom defined class 
    to established connection in your project
