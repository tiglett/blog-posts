# Weekly update [18/11/2013]
This week I created the IWalkInterface prototype and a skeleton IPointOfInterest interface. The IWalkInterface contains:
        public void addPOI(IPointOfInterest point);
        public void cancelWalk();
and the IPointOfInterest is empty.
I also changed our github repository as it was set up to be a Java project rather than an Android project. This was a problem because you cannot change a project to be a different kind of project without modifying the eclipse .project file.
I decided to take the .project file off the .gitignore in order for people to simply clone the repo and import the project. It is important that we use the whole project folder in git rather than just the source code folder as we need to have synchronised Android manifest and resource files.
I’m still waiting on the other group members to create their prototypes, but if they are having difficulties then it should be easy to resolve any issues and quickly finish these prototypes.

Hours spent this week:

 * Internal meeting: 1 hour
 * Interface Prototype and github refactoring: 1 hour
 * Total this week: 1 hours
 * Total so far: 11 hours
