Build Health
A 1-2 Year Plan for the LSE / POC / CMS Pod

Executive Pitch Summary
As our catalog scales, the LSE, POC, and CMS pod carries a growing production and quality burden with a lean team. Today, quality assurance and accessibility checks happen manually and after a course is built, and reusable components and automation exist at individual initiative rather than team standard. Our existing Tableau reporting covers student completion, engagement, and assessments, but not build-level technical or accessibility health.
Build Health closes that gap with three connected pieces: an automated quality and accessibility gate that catches defects before launch, a technical and accessibility health feed that extends our existing Tableau reporting to cover build-level quality rather than just student outcomes, and a team-standard reusable component and automation library that reduces variance and speeds every build.
This is the next stage of the value stream mapping work already underway on this team. Where a process map identifies where time and quality are lost, Build Health is the engine that acts on those findings continuously, without waiting for the next manual audit.
Over two years, this plan aims to cut pre-launch defect rates, reduce manual QA cycles per build, give leadership one place to see both student outcomes and build health instead of two separate pictures, and build a documented career-growth structure for a team of three distinct disciplines.
 
1. Context and Problem Statement
•	Academy's OKRs call for a scalable design system, a faster Alpha-to-Bravo lifecycle, and explicit portfolio health monitoring as the catalog grows. All three land directly on this pod's day-to-day work.
•	Quality and accessibility checks are currently manual and reactive. A recent WCAG audit on a live course unit found a critical focus-indicator gap and two major issues (unlabeled interactive elements, a data table missing scope and caption) after the course was already built and live.
•	The Live View student-facing environment has proven unstable during QA sessions, which pushes more of the burden onto direct DOM-level checks and away from relying on the student-facing environment to catch issues.
•	Reusable components and Python automation exist, but as individual initiative goals rather than a documented, versioned team standard. That means the benefit caps out at one person's output instead of the whole pod's.
•	The team already has shared Tableau reporting, owned by the data/BI team, covering student completion, engagement, and assessment activity. It does not yet cover build-level technical or accessibility health, Alpha vs. Bravo stage, or QA status. That picture still lives in people's heads or ad hoc requests.
2. Signature Initiative: Build Health
Build Health is a three-part system. Each part reinforces the others; together they turn quality and production work from a series of manual, one-off efforts into a standing team capability.
2.1 Automated Quality and Accessibility Gate
Convert the manual WCAG and technical QA audit process into a repeatable, automated pre-launch check, extending the JavaScript-injection DOM check method already validated on this team. The gate checks focus indicators, accessible names on interactive elements, table scope and caption presence, and other recurring issue patterns, before a course reaches CMS for final review or a student ever sees it.
Working theory: this does not replace CMS's judgment on content and instructional quality. It removes the class of technical and accessibility defects that are mechanical to detect, so CMS time shifts toward judgment calls that actually need a person.
2.2 Technical and Accessibility Health Feed (Extending Existing Tableau Reporting)
Rather than stand up a parallel dashboard, this extends the team's existing Tableau reporting, in partnership with the data/BI team that owns it. Today that reporting covers student completion, engagement, and assessment activity. This adds the technical and accessibility side of portfolio health: Alpha or Bravo stage, last QA date, outstanding accessibility or technical debt, and build owner, feeding in automatically from the gate in 2.1. That gives leadership and the Product Operations Coordinator one place to look for both student outcomes and build health, instead of two separate pictures, and answers OKR 5's call for visible impact without adding a second tool or a standing status meeting.
2.3 Reusable Component and Automation Library
Take the interactive components and Python automation already being built at the individual level and formalize them into a documented, versioned library with adoption tracking. This is the standard every LSE builds against and every CMS review checks against, so build speed and defect rate stop depending on which person built which course.
2.4 How the pieces connect
•	The component library reduces the defects the gate would otherwise have to catch.
•	The gate's pass/fail data feeds directly into the existing Tableau reporting instead of requiring manual status updates or a second tool.
•	The extended reporting's portfolio-wide view tells the team which offerings or components to prioritize next, closing the loop back to the library.
3. OKR Alignment
Initiative Component	OKR Alignment
Automated Quality and Accessibility Gate	OKR 3 (portfolio quality, automation) / OKR 4 (removing technical and process friction for students)
Technical and Accessibility Health Feed	OKR 3 (portfolio health monitoring, explicitly named) / OKR 5 (making impact visible)
Reusable Component and Automation Library	OKR 1 (scalable design system) / OKR 2 (rapid Alpha-to-Bravo build speed)
People and Growth Plan (Section 5)	OKR 5 (ownership, experimentation, growth of people as leaders and creators)
 
4. Roadmap
Year 1
Q1: Baseline and Alignment
•	Audit current LSE, POC, and CMS workflows end to end at the pod level, extending the team's existing value stream mapping work.
•	Define the technical and accessibility health fields to add to existing Tableau reporting, together with POC, the data/BI team that owns Tableau, and senior leadership input.
•	Inventory existing reusable components and automation scripts already built across the team.
•	Set baseline numbers: average QA cycles per build, average accessibility issues found post-launch, average build time.
Q2: Build MVPs
•	Ship v1 of the automated accessibility and QA gate for one course type.
•	Partner with the data/BI team to add a v1 technical and accessibility health view to existing Tableau reporting; manual data entry acceptable at this stage.
•	Formalize the component library structure and migrate the first three reusable components into it.
Q3: Adopt and Iterate
•	Roll the gate out to all active LSE builds.
•	Train CMS to use gate output as a starting point rather than a full manual re-audit.
•	Train POC to use the extended Tableau view for cross-department reporting instead of ad hoc status requests.
•	Iterate on the gate's false positive and false negative rates based on real usage.
Q4: Prove Impact
•	Present time saved, pre-launch vs. post-launch defect counts, and adoption rate of the new Tableau fields to leadership.
•	Identify next-year automation targets based on the data gathered, not assumption.
Year 2
Q1-Q2: Scale
•	Extend the gate and the Tableau health feed to Bravo-stage products and full cross-team visibility.
•	Connect the demand and completion signals already in Tableau to the new technical and accessibility fields, so OKR 2 and OKR 4 data sit in the same view as build health.
•	Stand up a leveling and growth framework across the three disciplines on the team.
Q3-Q4: Institutionalize
•	Full technical and accessibility health reporting live across the catalog, integrated into existing Tableau infrastructure.
•	Formal mentorship and coaching cadence in place, tied to performance review cycles.
•	Report year-over-year metrics on production speed, defect rate, and accessibility outcomes.
•	Propose the Year 3 roadmap based on what the data shows worked and what did not.
 
5. People Leadership Plan
A process and tooling plan on its own does not satisfy the leadership expectations of this role. This section covers the people side directly.
•	Standing 1:1 cadence with each of the 8-10 direct reports across three distinct disciplines, with a skills matrix specific to each role (LSE, POC, CMS) to guide coaching conversations.
•	Mentorship structure pairing experienced LSEs with newer hires on component and automation work, so the library in Section 2.3 also functions as a teaching tool.
•	Growth conversations tied to the same OKR-linked, quarterly goal structure already used on this team, giving each person a clear line from their work to team and company OKRs.
•	Change management approach: co-design the gate's check rules and the new Tableau fields with the team building them, rather than handing down a finished tool. Adoption is higher when the people using a system helped define it.
•	Headcount and backfill posture as the catalog scales: raise resourcing needs with the Senior Manager based on Tableau data on team capacity, rather than anecdote.
•	Build and maintain a working relationship with the data/BI team that owns Tableau reporting. This initiative depends on their partnership and capacity, not on working around them.
6. Success Metrics
Metric	Baseline (End of Q1, Yr 1)	Target (End of Yr 2)
Pre-launch defect rate (accessibility + technical)	Establish from Q1 audit	Meaningful reduction from baseline
Manual QA hours per course build	Establish from Q1 audit	Reduced through automated gate
Adoption of new technical/accessibility fields in Tableau (active weekly use by POC/leadership)	0 (fields do not yet exist)	Standard part of portfolio review
Reusable components in team library	Individual, undocumented	Team-standard, versioned library in active use
Team growth: documented skills matrix and 1:1 cadence	Not yet formalized	Fully in place for all direct reports
7. Risks and Open Questions
Flagged here as working theories, not settled conclusions. Each needs validation before full commitment.
•	This plan depends on the data/BI team's capacity and willingness to add new fields to existing Tableau reporting. That needs to be scoped as a partnership in Q1, not assumed as a given.
•	Automated checks will not replace all human QA judgment. The exact split between automated gate coverage and CMS's manual review scope needs to be worked out with the CMS role directly, not decided for them.
•	Live View platform instability is outside this pod's control. The plan leans on direct DOM-level and Studio-side checks specifically because of this, but platform reliability remains a dependency worth flagging upward.
•	Tooling investment (time and any budget) for building the gate and the Tableau integration needs Senior Manager sign-off before Q1 work begins in earnest.
