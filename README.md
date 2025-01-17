# FrameAR (Winner at EngHacks 2019)

![Cruise Model](https://raw.githubusercontent.com/rushigandhi/FrameAR/master/graphics/boat.jpg "Cruise Model")

[Check out the project on Devpost](https://devpost.com/software/framear)

## Inspiration

Despite there being 40 million Sketckup, Maya and 3D software users in an industry worth over \$56 billion, mechanical engineers, architects, designers, etc, lack a way to instantly display and receive live edits on their 3D renderings or experience the full power of version control that us software engineers are so familiar with. FrameAR is a multi-platform application that fills this gap through the creation of a version control system where users can track live commits in slack and instantly view edits and their models in augmented reality with the full power of branches, comparisons and merging from the VCS. FrameAR looks to provide creative teams new and dynamic means of collaboration to interact with the newest, greatest technologies.

## Brief Description of Project

Backend ( Kotlin, SpringBoot ) : FrameAR's stack starts with its Kotlin/SpringBoot backend server that allows us to track commits, branches, comments, users and more. The back handles the majority of the file handling and includes the vital conversion of the users STL files into a SCN files which is passed into the design and AR views.

Web View (React.js, stdlib): Instead of relying on the terminal and complicated Git commands, we wanted our non-technical audience to experience version control through a painless web api. Users have the full functionality of git from which they can make commits, create branches, merge branches and view all their comments. The view also renders a dynamic Git tree that allows users to visually track their projects progress. This data is passed along to the slack-bot which keeps track of the commit history in a slack channel in order to improve collaboration and decrease the likely-hood of errors. The Slack bot also incorporates deep-linking to allow users to open their projects at exact commits or branches into the AR view.

AR View ( AR-kit, Swift ) : The FrameAR iOS app renders SCN files of any of the users commits from any branch or project. The app creates pixel perfect AR models that can be resized, rotated and viewed from the inside and the outside. They can add comments at specific locations of the model and compare the differences between two commits and open multiple project files in the same world. By communicating with the backend, we not only user and commit files but also can register comments in the backend.

## What's next for FrameAR

In the future we hope to see our idea implemented in real workplaces in the future. This includes creating a similar project community similar to GitHub, more animated/interactive AR features, version control insights and improved, real-time collaboration methods. We hope to further polish our features for usage in industries such as AR/VR gaming, construction & architecture and entertainment

## Checkout the demo video here:

[https://www.youtube.com/watch?v=GG4c6HUJOf8](https://www.youtube.com/watch?v=GG4c6HUJOf8)

[![FrameAr Demo Video](http://img.youtube.com/vi/GG4c6HUJOf8/0.jpg)](https://www.youtube.com/watch?v=GG4c6HUJOf8)
