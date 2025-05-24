











IFB240 Cyber Security
Lecture 5 - Part B
Major Access Control Approaches
Dr Leonie Simpson lr.simpson@qut.edu.au

Major access control approaches
• How will access control decisions be made?
• Three major approaches
- Discretionary access control
• Decision at the discretion of some individual, possibly the
information asset owner
- Mandatory access control
• System wide set of rules applied
- Role-based access control
• Access permissions based on the role of the individual, rather than the individual identity (roles include user, administrator, student, etc)

Basic access control concepts
• Access control terminology
- Subjects
• Entities requesting access to a resource
- Examples: Person (User), Process, Device
• This is an active role
- Entity initiates access request and is user of information/resource
- Objects
• Resources or entities which contain information
- Examples: Disks, files, records, directories
• This is a passive role
- Object is repository for information or the resources that a subject tries to access

Discretionary access control (DAC)
• Access rights to an object or resource are granted at the discretion of the owner
• For example, the security administrator, the owner of the resource, or the person who created the asset
- DAC is discretionary in the sense that a subject with a certain access authorization is capable of passing that authorization (directly or indirectly) to any other subject
- Often implemented in access control lists (ACL) or matrices
- May be used to control access to resources such as
• Files or directories
• Networks

Discretionary access control
• Example: Sharing OneDrive files or folders
- For a particular object
• Locate object
• Right click on object
• Choose Sharing, and
• Enter the name of a user or group to share this with
• Then Send

Discretionary access control
• Example: DAC in Unix
- Object on each line
- Permissions indicated for: Owner, Group and Other
- Type of permissions: r read, w write and x execute
- Can use chmod command to change file access permissions


Mandatory access control
• A central authority assigns attributes to objects and to
subjects
- Example:
• subjects assigned clearance levels,
• objects assigned classification levels
• Have a system-wide set of rules relating
- attributes of the objects and subjects to
- the modes of access that are permitted

• MAC is mandatory in the sense that entities are not able to decide which other entities they want to allow to access resources, the system rules apply
- the system denies users full control over determining who gets access to the resources they create

Mandatory access control
Example - BLP model security level hierarchy
Top Secret
?
Secret
?
Confidential
?
Classified
?
Unclassified

Mandatory access control
Example: BLP model - mandatory access control
Compare subject clearance with object classification to determine

Secret






Secret

Secret

Role-based access control
• Access rights are based on the role of the subject, rather than the subject's individual identity
- A role is a collection of procedures or jobs that the subject performs
• Examples: user, administrator, student, etc
- A subject could have more than one role
• Example: Tutor may be a student and also a staff member
• But can only be acting in one role at any particular time
- More than one subject could have the same role
• Example: Lots of students!

• IMPORTANT: any subject can only perform in one role at any particular point in time

Role-based access control
• Example: 'Canvas' defined roles
• Source: Access and roles in Canvas - Staff - QUT Portal

Combining access control approaches
• Can use combinations of access control approaches
- Example: Combining mandatory and discretionary access control approaches
• Mandatory access control is applied first
• If access is granted by the mandatory access control rules,
then the discretionary system is invoked
• Access granted only if both of the approaches permit access
- Combining mandatory and discretionary access control approaches ensures that
• no owner can make sensitive information available to unauthorized users, and
• 'need to know' can be applied to limit access that would
otherwise be granted under mandatory rules
- Other combinations possible: RBAC with DAC or MAC

Summary
• Access control is important for information security
• Need to know
- what your information assets are, and
- where they are located
- how sensitive/critical they are
- Who needs access to each resource, and what mode of access
• Consider how access control policy decisions will be made
• Major access control approaches
- Discretionary
- Mandatory
- Role-based


