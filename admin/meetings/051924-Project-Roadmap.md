# CSE 110 Team 35 Meeting #7 - Project Roadmap

## Overview
- **Team Number**: 35
- **Meeting Type**: Regularly Scheduled
- **Location**: Online
- **Objective**: Prepare for the final project: Initial Pitch
- **Time**: 1:30 PM - 2:30 PM, May 19, 2024

## Attendance

### Leader
- [X] Allen Zhang
- [X] Shota Yasuraoka

### Member
- [X] Andrew Tan
- [ ] Anny Zhao
- [X] Audrey Liang
- [ ] Ethan Lee
- [ ] Ivor Myers
- [X] Jonathan Zhang
- [X] Mitchell Bizzigotti
- [ ] Tyler Khuc
- [X] Vincent McCloskey

## Agenda

### Unfinished Business from Last Meeting
None

### New Business to Cover
- [X] Discuss library / framework / tool usage expectation
- [X] Discuss project roadmap

## Decisions

### Task
- `id` - to uniquely identify the task
- `title` - title of the task
- `description` - description
- `priority` - priority
- `status` - status
- `createdAt` - start date
- `dueAt` - due date

### Journal
- `id` - id
- `title` - title
- `path` - journal folder -> file path
- `content` - markdown content
- `tags` - tags
- `createdAt` - created date

### TaskJournal (many to many relation)
- `journalId`
- `taskId`
