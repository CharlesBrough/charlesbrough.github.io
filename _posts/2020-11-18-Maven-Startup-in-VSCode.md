---
layout: post
title: Using Maven to start a Project in VSCode
---

# Starting a Maven Java project inside VSCode!

## Prerequisites

The Java extension suite must be installed to do this through the GUI.

### Step 1

Start in the directory where you want your project to go. Open the Maven panel as shown here and click the Add (plus-sign) button circled in red. (.metadata is from STS workspace)

![Screenie_1]({{ site.baseurl }}/images/maven-vscode-post/sc1.png)

### Step 2

Next, you’ll need to go through a couple of menus at the top. Since we’re doing Java 8, I used this:

![Screenie_2]({{ site.baseurl }}/images/maven-vscode-post/sc2.png)

### Step 3

This is the version of the Maven archetype we just selected, I just used the latest version:

![Screenie_3]({{ site.baseurl }}/images/maven-vscode-post/sc3.png)

### Step 4

This dialog will pop up asking to select where the project will be generated:

![Screenie_4]({{ site.baseurl }}/images/maven-vscode-post/sc4.png)

### Step 5

Now the rest of the setup is done through the VSCode console:
I filled in each of the 4 fields and I’m about to submit the last one above.

![Screenie_5]({{ site.baseurl }}/images/maven-vscode-post/sc5.png)

### Step 6

Then, simply confirm:

![Screenie_6]({{ site.baseurl }}/images/maven-vscode-post/sc6.png)

### Step 7: Done!

Here’s after build success:

![Screenie_7]({{ site.baseurl }}/images/maven-vscode-post/sc7.png)

That’s a VSCode generated Maven Java project! Develop away.

Alternative to this method would be using the command line ‘mvn’ command to generate the project, or using another IDE.

This method creates a somewhat large default pom.xml which includes a lot of base plugins and two dependencies related to JUnit. Creating an empty Maven project in STS is a bit cleaner, in my opinion, but this is totally valid as well.
