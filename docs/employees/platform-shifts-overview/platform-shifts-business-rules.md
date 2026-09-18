---
title: Shifts and time entries business rules
excerpt: >-
  The Toast platform applies the following business rules to shifts and time
  entries:
hidden: false
metadata:
  description: >-
    The Toast platform applies the following business rules to shifts and time
    entries:
---

The Toast platform applies the following business rules to shifts and time entries:

- *Time and order:* Clock-in time must be before clock-out time. A completed shift cannot be longer than 24 hours.
- *Overlapping shifts:* An employee cannot have two shifts whose worked times overlap. The Toast platform does not allow overlapping clock-in/clock-out periods for the same employee.
- *Breaks:* Every break must be fully within the clock-in to clock-out period for a time entry. Breaks cannot overlap each other. A completed shift cannot have a break that is still in progress; all breaks must have an end time before the shift is finished.
- *Job:* If the employee has at least one job assigned, the shift must specify which job they are working. The job must be one of the jobs assigned to the employee.
