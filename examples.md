# Clones, mirrors, forks, and such.

In open source software projects a fork is created when someone makes a copy of the code to start independent development on it. Free and open-source software is that which, by definition, may be forked from the original development team. In open source projects, forks are often used to work on new features before they are offered back to the community as a pull request. The 'fork and pull request' approach reduces friction for new contributors as it enables independent work with minimal upfront coordination. This makes for speedy collaboration on projects using a repo hosting service such as gitlab or launchpad which make it easy to Fork, Compare, and Pull Request with just a few clicks.


# RFC responsibilities

_Apperta **MUST** have a fork, clone, replica or snapshot of any/all code repositories at the point of completion of a project._

Here is an example of [mirroring](https://help.github.com/articles/duplicating-a-repository/#mirroring-a-repository) a github based project to the Apperta Foundation organisation
```
git clone --bare https://github.com/NeovaHealth/openeobs.git
cd openeobs.git
git push --mirror https://github.com/AppertaFoundation/openeobs.git
```

Here is an example of [mirroring and tracking](https://help.github.com/articles/duplicating-a-repository/#mirroring-a-repository-in-another-location) a github based project including getting updates from the original repo to the Apperta Foundation organisation
```
git clone --mirror https://github.com/NeovaHealth/openeobs.git
cd openeobs.git
git remote set-url --push origin https://github.com/AppertaFoundation/openeobs
```
