# OOS-MAIL
PL/SQL mail wrapper for APEX_MAIL with enhanced functionality.

This project is in the planning phase. It's goal is to support the following features:
- Wrapper for APEX_MAIL
  - Needs to support APEX 4.2 and 5.0 differences
    - Can do this with conditional compilation
- Priority queuing
  - Have a low/med/high level priority system.
- Dev/Test/Prod options
  - If not in production, add ability to differ mail to another address (i.e. never send an email to actual client unless we're in production).
  - Will need a configuration table to support where to send mail to and what function should be run to determine if we're in production or not
    - Prod fn can be a true/false since that's all we care about.
    - May want to factor in different levels of this (i.e. test can go to another system?)
