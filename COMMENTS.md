# Broader Comments

See my in situ comments throughout particular files. Extrapolate those comments and consider them throughout the model. Here are some other comments to consider.

## Information Architecture (IA)

### Folders-Files

I appreciate the thoughtfulness when it comes to your folder-file structure. However, consider how it is attuned a little too closely with the linearity of the procedures, which does not coincide with DITA topic modeling's focus on reuse. Specifically, each subfolder is a very specific procedure, `creating-a-new-save-procedure`, for example. 

Topic models must be architected for reuse, wherein there should never be a folder for every single procedure, as same activities may share content. I could see a potential idea where the IA is more general, such as `farming`, `avatars`, `general`, etc. But, for this "mini" assignment, I was really only expecting general folders like `tasks`, `concepts`, and `references` with the potential need for a `shared` topics folder.

In effect, your folder naming has gotten quite long, which can be cumbersome to use, which I'm sure you've noticed: 

- creating-a-new-save-procedure
  - creating-a-new-save-concepts
  - creating-a-new-save-references
  - creating-a-new-save-tasks

### Assets

Also, your assets should all be organized in the provided `assets` folder. Assets include images or other media files like documents of some sort. They should not be organized specific to 1 procedure. Again, think of reuse as the guiding principle. 

## MD Files

Please remove any files that are not a part of the topic model, such as the md files. I wish I would have reminded folks about the .gitignore file. You could have told git to ignore them and never actually version them. That would have been the move to make there. No worries. It's not graded per se, but the idea of superfluous files is definitely a concern to address for the final version of the project.

## Using Correct Topic Type

I offer comments in situ wherein I suggest that sometimes you are writing a task topic as a concept, and other times a reference topic material as a concept. Be sure to consider the appropriate semantics throughout.
