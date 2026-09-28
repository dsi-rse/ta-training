# TA Session Guide

This guide outlines best practices for running your two weekly TA sessions.  
Sessions are not traditional office hours — they are structured, working sessions where project teams make real progress under your supervision.  

## Purpose of TA Sessions
- Provide students with structured time to work on their project.  
- Ensure accountability: students attend, contribute, and meet milestones.  
- Help students debug technical issues without doing the work for them.  
- Reinforce best practices in software development and project management.  
- Serve as the first line of support before mentors and instructors.  

## Expectations
- Duration: 1 hour, twice per week.  
- Attendance: Required for students; report weekly in Canvas.  
- Format: Active working session, not passive Q&A.  
- Role: Guide, troubleshoot, and enforce good practices.  
- TA sessions are where debugging happens. Mentors are instructed not to debug code during the mentor meeting, so expect that work to be your responsibility.  
- A student with no pushed code by midnight before the mentor session receives a 0 for the week. This session is where you catch that.  

## Structure of a Typical Session
1. **Check-in (5–10 min)**  
   - Take attendance.  
   - Ask each student what they are working on this week.  
   - Review the status of pull requests and reviews.  
   - For students without active pull requests, review task status and path to completing the task this week.  

2. **Work Period (40–45 min)**  
   - Circulate among students, checking progress.  
   - Help debug technical issues (Git, Python, Docker, Make).  
   - Review open pull requests (with the `/clinic-pr-review` skill if you find it useful), then leave your review on the pull request.  
   - Encourage collaborative problem solving.  

3. **Wrap-up (5 min)**  
   - Summarize what was accomplished.  
   - Identify blockers for next session.  
   - Remind students of upcoming deadlines (weekly issues and reports, deliverables, client presentations).  
   - Enter attendance grades in Canvas.  

## Your Role During Work Periods
- **Guide, don’t solve:** Ask questions that lead students to the solution.  
- **Reinforce best practices:** Encourage good commits, documentation, and testing.  
- **Keep teams accountable:** Make sure everyone is contributing.  
- **Prioritize workflow issues:** Spend time on Git conflicts, PR reviews, and repo management.  

## Common Scenarios
- **Merge conflicts** → Walk through resolving conflicts and explain strategies to avoid them.  
- **Messy or undocumented code** → Point students to style guides and insist on docstrings/comments.  
- **Environment issues (Docker, Python)** → Help diagnose but encourage students to maintain reproducible environments.  
- **Students not engaged** → Pull them into conversation, assign them a task, or flag to mentor if persistent.  
- **Setup still broken** → Escalate to clinic RSE / technical staff in the mentor-TA Slack channel. If a student can't get their computer set up for a week, that's already ~12% of work time wasted.  
- **Struggling with the problem, not the code** (not understanding the data, failure to normalize or contextualize data, the same task repeated over and over) → Help with these issues when possible, but it can be difficult as a TA to gain a deep understanding of the data and other elements of the content. If students are struggling with these issues, notify the mentor and technical advisor.  

## Do’s and Don’ts
**Do**  
- Encourage teamwork and collaboration.  
- Provide actionable feedback during code reviews.  
- Ensure students are using reproducible workflows.  
- Report attendance weekly and flag issues quickly.  

**Don’t**  
- Complete deliverables for students.  
- Ignore unprofessional or disengaged behavior.  
- Allow students to skip best practices for the sake of speed.  
- Debate grades or exceptions — refer to the clinic director.  

## Weekly Checklist
- [ ] Held two sessions.  
- [ ] Reported attendance in Canvas.  
- [ ] Confirmed every student is pushing to GitHub, opening pull requests, and opening issues.  
- [ ] Reviewed open PRs and left reviews.  
- [ ] Escalated technical issues to clinic RSE / technical staff and other student concerns to the mentor.  
- [ ] Posted a weekly update for each project to the thread in the clinic TAs Slack channel: Are any students not pushing code or putting work in issues? Are you caught up with reviews? Are students blocked by anything in particular? Anything to escalate?  

See the clinic's [How to Run a TA Session](https://clinic.ds.uchicago.edu/mentor-ta/how-to-run-a-ta-session.html) checklist.
