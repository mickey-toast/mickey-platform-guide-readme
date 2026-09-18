---
title: Shifts overview
excerpt: >-
  A shift is a record of the time that an employee clocks in and works at a
  Toast platform location.
hidden: false
metadata:
  description: >-
    A shift is a record of the time that an employee clocks in and works at a
    Toast platform location.
---

A shift is a record of the time that an employee clocks in and works at a Toast platform location.

**Examples of information stored in a shift record**

- The record of the time that the employee *actually worked* at the location.
- The identifier of the employee and the job assignment for the shift.
- The date and time employee clocked in and clocked out.
- The location that the employee clocked in and clocked out at.
- The job assigned for the shift.
- Information about breaks during the shift.

A *time entry* is the record of work for a shift. You can review the time entries for employee shifts in Toast Web on the **Time entry management page**. For more information about time entries, see [Time entries and breaks](https://doc.toasttab.com/doc/platformguide/platformShiftsTimeEntriesAndBreaks.html).

The Toast platform creates a time entry when an employee clock in. After the employee clocks out, they cannot edit the time entry. Only a manager can correct a time entry after the employee clocks out.

Each shift is assigned to a business day. The business day for a shift is determined by the shift start time and the business day cutoff time for the location. For example, if a location has a business day cutoff time at 4:00 a.m., a shift that starts at 2:00 a.m. is assigned to the business day that is ending (the previous calendar day for reporting).

You can create scheduled shifts to use with schedule enforcement for employees. Scheduled shifts record a plan for an employee's shift and are different from a shift that records an employee's clocked in work. For more information, see [Scheduled shifts for schedule enforcement](https://doc.toasttab.com/doc/platformguide/platformScheduledShifts.html).
