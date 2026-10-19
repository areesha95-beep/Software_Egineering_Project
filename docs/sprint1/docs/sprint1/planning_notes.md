# Sprint 1 Planning Notes

* Date:                      Monday, 19 October 2026
* Meeting Type:              Sprint Planning 
* Team:                      Laraib Samreen (Scrum Master), 
                             Javeria Ahmad (Product Owner), 
                             Shamin Bibi (Dev),
                             Areesha Naeem (Dev)
* Total Points Committed:    31 Points

### (Sprint Goal):
We want a simple working version from start to finish:
A user types a hardware request in plain English, Gemini generates the Verilog code, our Python script saves the `.v` file, Icarus Verilog compiles it and we see a clear PASS or FAIL in the terminal.

### Key Discussion & Decisions:
1. We will not try to build all 6 agents right now. For Sprint 1, we only focus on two things:
   - Shamin builds the RTL generator agent.
   - Areesha builds the Icarus Verilog test runner.
   The remaining agents (repair loop, testbench generator) stay in the backlog for Sprint 2.
2. No one pushes straight to `main`. Everyone creates a branch named `feature/SCRUM-xx`, opens a pull request, and gets at least one review before merging.
3. We will do a quick 10-minute sync every day at 2:00 PM to check progress and blockers.

### Task Distribution:
* Javeria (5 pts): Backlog stories, Acceptance Criteria, Definition of Ready / Done.
* Shamin (10 pts): Gemini API connection wrapper, versioned prompt v1.0, RTL generator script.
* Areesha (9 pts): Icarus Verilog execution script, CLI entrypoint (`main.py`), unit tests.
* Laraib (7 pts):  Prompt test suite (5 test cases), hallucination checklist, daily burndown tracking, traceability sheet.