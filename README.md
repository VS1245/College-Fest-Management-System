# College Fest Management System

## Introduction
This C++ program implements an object-oriented approach to managing a college fest. It includes classes for Students, Logistics, Treasury, Website, WorkforceMember, Coordinator, CoreMember, Event, and Participant. These classes form the foundation for organizing and participating in college fests.

## Classes

### Student
- **Attributes:**
  - `Id` (int): Unique identifier for each student.
  - `Name` (string): Student's name.
  - `Email` (string): Student's email address.

- **Methods:**
  - `setId(int id)`: Sets the student's ID.
  - `setName(string name)`: Sets the student's name.
  - `setEmail(string email)`: Sets the student's email.
  - `getId()`: Returns the student's ID.
  - `getName()`: Returns the student's name.
  - `getEmail()`: Returns the student's email.

### Logistics
- **Methods:**
  - `Logistics(string name)`: Prints the manager’s name.

### Treasury
- **Methods:**
  - `Treasury(string name)`: Prints the manager’s name.

### Website
- **Methods:**
  - `Website(string name)`: Prints the manager’s name.

### WorkforceMember
- **Attributes:**
  - `Role` (string): Role assigned to the workforce member (e.g., logistics, treasury, publicity).
  - `taskAssigned` (string): Task assigned to the workforce member.
  - `taskCompleted` (bool): Flag indicating whether the assigned task is completed.

- **Methods:**
  - `assignRole(string role)`: Assigns a role to the workforce member.
  - `getRole()`: Returns the role assigned to the workforce member.
  - `performTask()`: Marks the task as completed for the workforce member.
  - `assignTask(string task)`: Assigns a task to the workforce member.
  - `markTaskCompleted()`: Marks the assigned task as completed.

### Coordinator
- **Attributes:**
  - `Workforce` (vector<WorkforceMember*>): List of workforce members.

- **Methods:**
  - `assignTaskToWorkforce()`: Assigns a task to the workforce member.
  - `reportToCoreMember()`: Returns the role assigned to the core member.
  - `addWorkforceMember(WorkforceMember* workforceMember)`: Adds a workforce member under the coordinator.

### CoreMember
- **Attributes:**
  - `specialization` (string): Area of specialization (e.g., logistics, treasury, website).

- **Methods:**
  - `setSpecialization(string specialization)`: Sets the core member's specialization.
  - `getSpecialization()`: Returns the core member's specialization.
  - `getCoordinators()`: Returns the list of coordinators reporting to the core member.
  - `addCoordinator(Coordinator *coordinator)`: Adds a coordinator to the core member's team.
  - `removeCoordinator(Coordinator *coordinator)`: Removes a coordinator from the core member's team.

### Event
- **Attributes:**
  - `eventId` (int): Unique identifier for each event.
  - `eventName` (string): Event's name.

- **Methods:**
  - `getEventId()`: Returns the event id.
  - `getEventName()`: Returns the event’s name.

### Participant
- **Attributes:**
  - `eventsParticipated` (vector<Event*>): List of events in which the participant has participated.

- **Methods:**
  - `getEventsParticipated()`: Returns the events participated by the participant.
  - `participateInEvent(Event *event)`: Adds an event to the list of events participated by the participant.
  - `withdrawFromEvent(Event *event)`: Withdraws the participant from a specific event.

## Usage
- Create instances of the classes to manage students, coordinators, events, and participants.
- Use the provided methods to interact with the objects and perform various tasks related to fest management.

Feel free to extend the functionality as needed for your college fest management system.
