# TeMe77 = Teemu Merisalo / 7boddy = Jussi Kivistö
## ELT-53108-Exam-Task5
ELT-53108 Computer Networking II, Exam Task 5, Merisalo &amp; Kivistö

You may work in groups of up to 3 people, if you do so the assignment number is calculated by adding all IDs together and then taking mod 6 to get the assignment number . Group work must be clearly indicated in submission, all members of the group will receive the same grade irrespective of the contributions made by each individual. Any group work must be carried out with version control, such that author identity may be clearly tracked throughout the project history (in case of plagiarism etc). You may use github or TU git repositories for that, as long as full VCS history is made available to the teacher. Individual contribuitions do not have to be version control tracked, but doing so may be a good idea anyway. You will have to do the reviews individually (even if you act as a group for primary submission).

You will have plenty of time to complete the tasks, but doing them on the last day before deadline is ill advised.

The main submission should be formatted according to the general outline of RFC specifications ( https://www.rfc-editor.org/styleguide/ ), you can use relevant templates and tools from https://www.rfc-editor.org/pubprocess/tools/ . As such, your initial submissions will effectively be going through a process similar to that for RFCs. Unlike "normal" RFC process, I further encourage usage of graphical materials in your specifications where appropriate (you may refer to https://tools.ietf.org/id/draft-rfc-image-files-00.html for style guide on that). It is extremely helpful to use PlantUML to make systematic and nice diagrams for protocols and packet exchanges https://plantuml.com/.  It helps to visualize packet exchanges as message sequence charts, while signals and timers can be visualized as UML/SDL diagrams in a very easy manner. Keep your proposal under 10000 characters of text at all times. Do not submit any non-text files (other than graphics), usage of pdf/word or other complex format will disqualify your submission.

Final submission should be made as a zip or tar.gz archive with no password, and for group work this must include .git directory for version control tracking you have used. Your submissions should not include ANY OTHER identification at all (such as your names or student IDs) anywhere outside .git directory, such that anonymous peer review can be organized. Moodle keeps track of who sent which file, so do not worry that your works will get misplaced.

Task 5: Submarine communications (latency)

In a dystopian far future humanity had to move to the deep underwater to avoid horrible pollution on the surface. All satellites have been lost due to massive amount of debris in orbit. While major settlements are connected with fiber, small submarines and people working underwater still need to talk. Luckily, WiFi appeared to work mostly unchanged, but its range was greatly limited to about 10m.  However, a variant of cellular network was needed that would work well underwater at longer ranges, up to 1 kilometer. As such, it would need to rely on ultrasound as physical layer. There are two specific issues with that:
 * Speed of sound is very low compared to light speed, which delays any signaling from base station to mobile device a lot
 * Bandwidths are very limited (64 frequency channels of 8 kbps each), so only voice communications are possible
 You need to consider the protocols that would handle signaling related to association with base station, as well as handover from one base station to another (you may assume other procedures are taken care of). The network must be provisioned to support several users at the same base station at any given time.

