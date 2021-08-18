# Sales
This is a "Hello World" application which is designed to show the core capabilities and features of both the Jmix Framework and Studio.

The Sales application is a simple purchase management system that enables tracking orders made by customers. Each order consists of a number of products. Customers, products and orders can be created, edited and deleted through the system user interface.

The application project covers the following aspects:

- Data Model Design
  - Creating entities
  - Executing DDL scripts
  - Creating relationships in entities
- User Interface Design
  - Generating CRUD screens
  - Creating views for related entities
  - Creating data containers for screens to display composite screens
  - Visual editing of the existing screens
- Creating Integration Tests

Based on Jmix Framework 1.0.1

# Issues
Please use https://www.cuba-platform.com/discuss/c/jmix/40 for discussion, support and reporting problems corresponding to this sample.

### Instructions for Apache Directory Studio installing if it has not been installed yet
1. Download [here](http://directory.apache.org/studio/) and install Apache Directory Studio
2. Run Apache Directory Studio (ApacheDirectoryStudio.exe on Windows or ApacheDirectoryStudio on Linux)
3. Create new server using LDAP Servers tab:
4. Choose server type ApacheDS 2.0.0 and set server name -> Click Finish:
5. Invoke a server's context menu -> Choose Create connection:
6. Select server -> Run
7. Switch to Connections tab -> Invoke created connection's context menu -> Open connection:
8. Invoke context menu of tree item *dc=example, dc=com* -> New -> New Entry
9. Create entry from stratch -> Next
10. Choose object class 'inetOrgPerson' -> Add -> Next 
11. In RDN combobox select *cn* -> set any name to the text unput(**ldapuser** e.g.) -> Next
12. Set the same value to the **sn** field -> Finish
13. Invoke context menu from **sn** attribute -> New attribute
14. In Attribute type combobox select *userPassword* -> Next
15. Set password and password confirmation (please use any complicated value, like *11passwd11*)
16. Switch to Connections tab -> New connection
17. Set any name to Connection name field
18. In Hostname combobox select *localhost*
19. In Hostname combobox select *10389* -> Next
20. In Hostname Bind DN or user  select *cn=ldapuser, dc=example, dc=com* (*ldapuser* is created user name)
21. Set password to Bind password field -> Finish
22. Switch to LDAP Servers -> Click two times to created server
23. Deactivate Allow Anonymous Access checkbox -> press Ctrl + S
24. Set to **application.properties** created username and password


### Instructions for Apache Directory Studio running
1. Run Apache Directory Studio
2. Select server -> Run
3. Switch to Connections tab -> Select connection with custom name -> Open connection
4. Set to **application.properties** used username and password