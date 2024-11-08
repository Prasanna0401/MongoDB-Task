-- To create and use database:
```javascript
use databaseName
```

-- To create collection:
```javascript
db.createCollection("collectionName")
```

-- users Collection:
```javascript
[
    { "name": "Alice", "email": "alice@example.com", "codekata_solved": 15, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-02", "status": "absent" }], "mentor_id": "mentor1" },
    { "name": "Bob", "email": "bob@example.com", "codekata_solved": 25, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-05", "status": "absent" }], "mentor_id": "mentor1" },
    { "name": "Charlie", "email": "charlie@example.com", "codekata_solved": 10, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-03", "status": "present" }], "mentor_id": "mentor2" },
    { "name": "David", "email": "david@example.com", "codekata_solved": 5, "attendance": [{ "date": "2023-10-01", "status": "absent" }, { "date": "2023-10-04", "status": "absent" }], "mentor_id": "mentor2" },
    { "name": "Eva", "email": "eva@example.com", "codekata_solved": 20, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-06", "status": "present" }], "mentor_id": "mentor3" },
    { "name": "Frank", "email": "frank@example.com", "codekata_solved": 30, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-07", "status": "absent" }], "mentor_id": "mentor3" },
    { "name": "Grace", "email": "grace@example.com", "codekata_solved": 18, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-08", "status": "present" }], "mentor_id": "mentor4" },
    { "name": "Hank", "email": "hank@example.com", "codekata_solved": 12, "attendance": [{ "date": "2023-10-01", "status": "absent" }, { "date": "2023-10-09", "status": "present" }], "mentor_id": "mentor4" },
    { "name": "Ivy", "email": "ivy@example.com", "codekata_solved": 22, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-10", "status": "absent" }], "mentor_id": "mentor5" },
    { "name": "Jack", "email": "jack@example.com", "codekata_solved": 28, "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-11", "status": "present" }], "mentor_id": "mentor5" }
]
```

-- codeKata Collection:
```javascript
[
    { "user_email": "alice@example.com", "problems_solved": 15, "date": "2023-10-01" },
    { "user_email": "bob@example.com", "problems_solved": 25, "date": "2023-10-02" },
    { "user_email": "charlie@example.com", "problems_solved": 10, "date": "2023-10-03" },
    { "user_email": "david@example.com", "problems_solved": 5, "date": "2023-10-04" },
    { "user_email": "eva@example.com", "problems_solved": 20, "date": "2023-10-05" },
    { "user_email": "frank@example.com", "problems_solved ": 30, "date": "2023-10-06" },
    { "user_email": "grace@example.com", "problems_solved": 18, "date": "2023-10-07" },
    { "user_email": "hank@example.com", "problems_solved": 12, "date": "2023-10-08" },
    { "user_email": "ivy@example.com", "problems_solved": 22, "date": "2023-10-09" },
    { "user_email": "jack@example.com", "problems_solved": 28, "date": "2023-10-10" }
]
```

-- attendance Collection:
```javascript
[
    { "user_email": "alice@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-02", "status": "absent" }] },
    { "user_email": "bob@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-05", "status": "absent" }] },
    { "user_email": "charlie@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-03", "status": "present" }] },
    { "user_email": "david@example.com", "attendance": [{ "date": "2023-10-01", "status": "absent" }, { "date": "2023-10-04", "status": "absent" }] },
    { "user_email": "eva@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-06", "status": "present" }] },
    { "user_email": "frank@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-07", "status": "absent" }] },
    { "user_email": "grace@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-08", "status": "present" }] },
    { "user_email": "hank@example.com", "attendance": [{ "date": "2023-10-01", "status": "absent" }, { "date": "2023-10-09", "status": "present" }] },
    { "user_email": "ivy@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-10", "status": "absent" }] },
    { "user_email": "jack@example.com", "attendance": [{ "date": "2023-10-01", "status": "present" }, { "date": "2023-10-11", "status": "present" }] }
]
```

-- topics Collection:
```javascript
[
    { "topic_name": "Introduction to Programming", "date": "2023-10-01" },
    { "topic_name": "Data Structures", "date": "2023-10-02" },
    { "topic_name": "Algorithms", "date": "2023-10-03" },
    { "topic_name": "Web Development", "date": "2023-10-04" },
    { "topic_name": "Database Management", "date": "2023-10-05" },
    { "topic_name": "Machine Learning", "date": "2023-10-06" },
    { "topic_name": "Software Engineering", "date": "2023-10-07" },
    { "topic_name": "Mobile App Development", "date": "2023-10-08" },
    { "topic_name": "Cloud Computing", "date": "2023-10-09" },
    { "topic_name": "Cybersecurity", "date": "2023-10-10" }
]
```

-- tasks Collection:
```javascript
[
    { "task_name": "Complete Assignment 1", "due_date": "2023-10-05", "submitted": false },
    { "task_name": "Project Proposal", "due_date": "2023-10-10", " submitted": true },
    { "task_name": "Midterm Exam Preparation", "due_date": "2023-10-15", "submitted": false },
    { "task_name": "Final Project", "due_date": "2023-10-20", "submitted": false },
    { "task_name": "Weekly Quiz", "due_date": "2023-10-07", "submitted": true },
    { "task_name": "Research Paper", "due_date": "2023-10-25", "submitted": false },
    { "task_name": "Group Presentation", "due_date": "2023-10-30", "submitted": true },
    { "task_name": "Code Review", "due_date": "2023-10-12", "submitted": false },
    { "task_name": "Feedback Session", "due_date": "2023-10-18", "submitted": false },
    { "task_name": "Final Exam Preparation", "due_date": "2023-10-28", "submitted": false }
]
```

-- company_drives Collection:
```javascript
[
    { "company_name": "Tech Corp", "date": "2020-10-16", "participants": ["Alice", "Bob"] },
    { "company_name": "Innovate Inc", "date": "2020-10-20", "participants": ["Charlie", "David"] },
    { "company_name": "Future Solutions", "date": "2020-10-22", "participants": ["Eva", "Frank"] },
    { "company_name": "Global Tech", "date": "2020-10-25", "participants": ["Grace", "Hank"] },
    { "company_name": "NextGen", "date": "2020-10-30", "participants": ["Ivy", "Jack"] }
]
```

-- mentors Collection:
```javascript
[
    { "name": "Mentor 1", "mentees_count": 20 },
    { "name": "Mentor 2", "mentees_count": 15 },
    { "name": "Mentor 3", "mentees_count": 10 },
    { "name": "Mentor 4", "mentees_count": 18 },
    { "name": "Mentor 5", "mentees_count": 25 },
    { "name": "Mentor 6", "mentees_count": 5 },
    { "name": "Mentor 7", "mentees_count": 30 },
    { "name": "Mentor 8", "mentees_count": 12 },
    { "name": "Mentor 9", "mentees_count": 8 },
    { "name": "Mentor 10", "mentees_count": 16 }
]
```

# Task Queries to Write:

-- 1. Find all the topics and tasks which are thought in the month of October:
```javascript
db.topics.find({ date: { $gte: "2023-10-01", $lte: "2023-10-31" } })
db.tasks.find({ due_date: { $gte: "2023-10-01", $lte: "2023-10-31" } })
```

-- 2. Find all the company drives which appeared between 15 oct-2020 and 31-oct-2020:
```javascript
db.company_drives.find({ date: { $gte: "2020-10-15", $lte: "2020-10-31" } })
```

-- 3. Find all the company drives and students who are appeared for the placement:
```javascript
db.company_drives.find({}, { company_name: 1, participants: 1 })
```

-- 4. Find the number of problems solved by the user in codekata:
```javascript
db.codekata.aggregate([
    { $group: { _id: "$user_email", total_problems_solved: { $sum: "$problems_solved" } } }
])
```

-- 5. Find all the mentors with who has the mentee's count more than 15:
```javascript
db.mentors.find({ mentees_count: { $gt: 15 } })
```

-- 6. Find the number of users who are absent and task is not submitted  between 15 oct-2020 and 31-oct-2020:
```javascript
db.attendance.aggregate([
    { $unwind: "$attendance" },
    { $match: { "attendance.status": "absent", "attendance.date": { $gte: "2020-10-15", $lte: "2020-10-31" } } },
    { $lookup: {
        from: "tasks",
        localField: "user_email",
        foreignField: "user_email",
        as: "task_info"
    }},
    { $match: { "task_info.submitted": false } },
    { $count: "absent_users_without_submissions" }
])
```