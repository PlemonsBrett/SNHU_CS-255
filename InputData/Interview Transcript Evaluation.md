# DriverPass Interview Transcript & Analysis

## Initial Client Meeting

### Attendees
<div style="color: #4A90E2"><b>Sam (System Analyst)</b> - Consulting Company</div>
<div style="color: #50C878"><b>Jennifer (Project Lead)</b> - Consulting Company</div>
<div style="color: #E67E22"><b>Liam (Owner)</b> - DriverPass</div>
<div style="color: #9B59B6"><b>Ian (IT Officer)</b> - DriverPass</div>

### Interview Content

<div style="color: #4A90E2"><b>Sam</b> Welcome, Liam and Ian. Liam, can you start by telling us a little about DriverPass? What is your vision for this company?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> I noticed that there is a need for better driver training. So many people fail their driving tests at the DMV. I'm starting this company to provide this type of training for my customers. I want them to be able to take online classes and practice tests. My company will also provide them with on-the-road training if they wish. I need you guys to help me build a system that will handle all of this.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Sounds great. What do you need from this system?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> I want the system to help me access my data from anywhere, online as well offline.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK. One thought. You can't modify or update the data unless you're online; otherwise, we might end up with duplicate data on different servers. This might cause data redundancy.</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Sure, sure—I knew that. That's what I meant. I want to access data online from any computer or mobile device. I need to be able to download the reports and some information that I can work on at home, using Excel, for example.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Absolutely. What about security?</div>
<br/>
<div style="color: #9B59B6"><b>Ian</b> We have different employees at the company with different rights and roles. For example, for me I need to have full access over all accounts so I can reset them if someone forgets their password, or if we let go of someone and I need to be able to block their access.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> What about tracking? Do you wish to know when a user makes a change to a record in the system?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Absolutely! For tracking, I need to make sure I know who made a reservation, who canceled it, who modified it last. All this must be clear in case something goes wrong. I want to be able to print an activity report and figure out who is responsible.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK. Can you tell me a little more about these reservations? What are the reservations for?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Our customers need to be able to make reservations for driving lessons. Each lesson is two hours long, and the customer should be able to tell us the day and time when they want to take that lesson. They should be able to make this reservation online using their account. Or they could call or visit our office to schedule an appointment with our secretary.</div>
<br/>
<div style="color: #E67E22">We also need to be able to identify the driver the customer is scheduled to go out with, since we have many drivers and many cars. We have to be able to track which user is matched up with a certain driver, time, and car.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK, great. How do the driving appointments work?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Sure. I have 10 cars. Each car has a driver. The customer can pick one of three packages:</
<br/>
- **Package One:** Six hours in a car with a trainer
- **Package Two:** Eight hours in a car with a trainer and an in-person lesson where we explain the DMV rules and policies
- **Package Three**: Twelve hours in a car with a trainer, an in-person lesson where we explain the DMV rules and policies—*plus* access to our online class with all the content and material. The online class also includes practice tests.
</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK. Anything else?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Yes. The way the registration should happen is that we get a phone call, and then the customer gives us their information. This information would include their first name, last name, address, phone number, state, and their credit card number, expiration date, and security code.</div>
<br/>
<div style="color: #E67E22">It should also include the pickup location from where the customer wants to be picked up. It should also ask them for a drop-off location, which should be the same as the pickup location.</div>
<br/>
<div style="color: #9B59B6"><b>Ian</b> As mentioned before, we also want the customer to be able to schedule appointments over the internet. If the customer forgets their password, we need them to be able to automatically reset it.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> What about compliance? How will you keep up-to-date with changes the DMV might make?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Oh, good question! We definitely want to make sure that the tests and practice we are providing are current with what the DMV requires. So we need to be able to be connected to the DMV so that they can update us with new rules, policies, or sample questions. We should get a notification whenever they have an update.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK, got it. What about the interface?</div>
<br/>
<div style="color: #9B59B6"><b>Ian</b> The system needs to run off the web, preferably over the cloud. We do not want to deal with backup and security; we need that to be taken care of. We need our focus to be on running the business with minimal technical problems.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK. What about look? Do you have any specific thoughts about the look of the interface, or do you wish us to come up with our own?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Oh, no—I do have a picture of what I want. Here, check this sketch out:</div>
<br/>
[Interface sketch showing layout with Logo, Online test progress, Information fields, Driver notes, Special needs, Driver photo, and Student photo]
<br/>
<br/>
<div style="color: #E67E22"><b>Liam</b> As you can see, the online test progress should show the tests the customer took. It should show what's in progress and the ones that the customer completed. So, it would say something like test name, time taken, score, and status. The status could be not taken, in progress, failed, or passed.</div>
<br/>
<div style="color: #E67E22">In the driver notes, I need to show any comments the driver left as well as the times for the lessons. So, it should show me something like this table:
<br/>

| Lesson Time | Start Hour | End Hour | Driver Comments |
|------------|------------|----------|-----------------|
|            |            |          |                 |
|            |            |          |                 |
</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> OK, so this is one of many pages we need to build, right?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> Absolutely. There should be an input form where the student (or secretary) fills in the student information, such as first name, last name, address, et cetera. There also should be a page for contacting us, and a way to contact the student.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Great. Any idea of what you might want to do in the future? Like future features?</div>
<br/>
<div style="color: #E67E22"><b>Liam</b> No, not yet. Let's focus on this; then maybe we can introduce new features to it.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Wonderful. I think we have enough here to get started. Sam and I will begin working on the system design and communicate this to our team. We will check in with you at different points to make sure that our design is meeting your needs. Thank you both for coming!</div>

## Project Planning Meeting

### Attendees
- <div style="color: #4A90E2"><b>Sam (System Analyst)</b></div>
- <div style="color: #50C878"><b>Jennifer (Project Lead)</b></div>

### Meeting Content

<div style="color: #50C878"><b>Jennifer</b> OK, Sam. How are we going to approach this?</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Well, I was thinking of laying out the tasks for this project. Then maybe we can arrange them according to dependency or importance. What do you think?</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> OK, Sam. How are we going to approach this?</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Well, I was thinking of laying out the tasks for this project. Then maybe we can arrange them according to dependency or importance. What do you think?</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Perfect. So we started this project by sitting with the client January 22nd and today is February 4th. That took 14 days for requirement collection.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Correct. So next, I think we should start building the use case diagrams and activity diagrams. If we start February 11th (since this week is a holiday), that should take us about eight business days.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> That's right. Meanwhile, we can at the same time have Toni and Clark research user interface designs. That should take them around nine days. Their task is not related to the use case diagram, so there is no dependency there.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Absolutely. Similarly, we can have John work on the class diagram. He needs nine days, and I know he's returning from his vacation March 1st. So he can start then.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Wonderful. We should be done by March 10th. Let's set that day and March 11th to meet with the customer to discuss the work with them.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Absolutely. Next, once the customer approves our work, and assuming he doesn't ask for modifications, we can start working on the interface March 12th. It will take us 12 days to complete. After that, we can build the database tables and link it to the interface. That should take nine days.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Correct. Once that's done, we need to add the business logic (security, role, right) layer, which will take 22 days.</div>
<br/>
<div style="color: #4A90E2"><b>Sam</b> Perfect. The system delivery will take a couple of days; then the sign-off meeting will take a couple of days as well.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Great. Here is the table I built based on what we discussed. I hope it helps.</div>
<br/>

| Task | Start Date | End Date |
|------|------------|----------|
| Collect Requirements | 22-Jan | 4-Feb |
| Create Use Case Diagrams | 11-Feb | 18-Feb |
| Build Activity Diagrams for Each Use Case | 15-Feb | 9-Mar |
| Research User Interface Designs | 27-Feb | 7-Mar |
| Build Class Diagram | 1-Mar | 9-Mar |
| Get Customer Approval | 10-Mar | 11-Mar |
| Build Interface | 12-Mar | 24-Mar |
| Link DB to Interface | 24-Mar | 3-Apr |
| Build Business Logic | 5-Apr | 27-Apr |
| Test System | 27-Apr | 7-May |
| Deliver System | 8-May | 9-May |
| Sign-off Meeting | 9-May | 10-May |

<br/>
<div style="color: #4A90E2"><b>Sam</b> Thanks. That works just fine.</div>
<br/>
<div style="color: #50C878"><b>Jennifer</b> Great! You can use this basic idea to create a GANTT chart for our documentation.</div>

## Key Requirements Analysis

### System Users
1. Owner (Liam)
   - Full system access
   - Reporting capabilities
   
2. IT Officer (Ian)
   - System maintenance
   - User access management
   - Password reset capabilities

3. Secretary
   - Appointment management
   - Customer registration
   
4. Instructors
   - Access to student information
   - Lesson scheduling
   
5. Customers
   - Online account access
   - Lesson booking
   - Access to learning materials

### Core System Requirements
1. Cloud-based web application
2. Role-based access control
3. Appointment scheduling system
4. Training package management
5. DMV integration for updates
6. Activity tracking and reporting
7. Mobile device accessibility

### Technical Considerations
1. Online-only data modification
2. Secure user authentication
3. Audit logging
4. Cloud-based security
5. Database integration
6. Interface customization
7. Payment processing

### Project Timeline
- Requirements Collection: Jan 22 - Feb 4
- System Design: Feb 11 - Mar 11
- Implementation: Mar 12 - Apr 27
- Testing: Apr 27 - May 7
- Deployment: May 8 - May 10