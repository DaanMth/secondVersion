## Before the sprint
Before we started the sprint we sat down with my stakeholders to indicate what we wanted to do next, as I wanted to make another functionality not knowing we didn't have that much time left my stakeholders had stated that it would maybe be a better idea to start fixing the bugs that are currenly still in the application and after that maybe work further on the last functionallity that they had in mind. They were pretty confident that I could work on this last functionality in this sprint, as it didn't really matter to them if it would be actually in the prototype or just something like a design. As long as I would do research on it and work it out in some sort of way they would be really satisfied. But first I started fixing the bugs that were still in the application and added some finsihing touches which I will elaborate more in the following paragraphs.

## Fixing bugs
The first bug that I fixed was one where I couldn't immediately put a component inside of the board, this caused me to recompile the whole application first before I could put a component inside of the board. I fixed this by changing the way I render the sidebar, first it rendered it every milisecond which caused it to give this priority. So I changed it that it only gets the sidebar the first time, this fixed the problem and I finally didn't have to recompile the application anymore.

----------------------------

![15c3846609dd15d12283e791c5ddd28a](uploads/767258b351a1a988cfd0bfeb63be2c6b/15c3846609dd15d12283e791c5ddd28a.gif)

----------------------------

The next thing that I wanted fixed was the fact that the current value didn't show up immediately, you first had to go out of the modal and go back in to see it. This happened because it was put inside of a UseState, and this only updates when the whole page gets rendered as a whole again. So this meant I needed to work around this to make it show up immediately. I did this by firing up another useState that is used as a decoy, I did this as my stakeholder gave me this tip a long time ago that this could work for some occassions. 

----------------------------

![a6fa5cf018733cabac910b9621d424d1](uploads/2c6534a28e2cbd246d81293498cb850e/a6fa5cf018733cabac910b9621d424d1.gif)

----------------------------

Another big bug that was still in the application was the fact that when you view a saved flow that it doesn't show the arrows that you had connected. This was caused because I only loaded the components that were on the board and I hadn't made a function yet that would generate the arrows that you also had connected to the components. So I started writing the function that saved the arrows to the backend as well and also the function that would load the arrows that you had connected.

----------------------------

![c37f7bff4f9df4191527c5627ffed1a9](uploads/dac6b6e6cbcd79e2107600bf1086c860/c37f7bff4f9df4191527c5627ffed1a9.gif)

----------------------------

Then I noticed that when viewing a saved flow with a custom component that it doesn't show that component but rather the components that are inside of it. This was caused because the function that I had originally written just loaded the functions that were inside of it rather than looking if it was a custom component. so I rewrote this function and this fixed the problem as a whole, this did cause for some extra bugs but those will be explained further below.

----------------------------

![f86ade4538f52e91021cc50df2e3c2d4](uploads/8cc6c4a110a930c00bfadf4cd20da331/f86ade4538f52e91021cc50df2e3c2d4.gif)

----------------------------

As I had fixed the fact that you could see the custom component in saved flows another bug had occured. Now I couldn't run the application anymore with custom components inside it and it only showed an error when running. After doing some research I had noticed that it didn't work because of the fact that I changed a few objects inside of the component to make the component visible in the saved flows. So after some changing here and there I made it work again. 

-----------------------------

![4afc3902d1de4b59e0f1626a1fc2ee2a](uploads/349367e1d5d3894108d45226625b94a9/4afc3902d1de4b59e0f1626a1fc2ee2a.gif)

## Finishing touches
As I wanted to add some more to the design I noticed that the pages were a bit static, when going from one to another it didn't flow well and the homepage was still kind of boring in my eyes. So I made the decision to add animations to the webpage. The homepage needed some more spice when first starting it and when going to other pages it should have that little detail that satisfies the user. So I ended up animating the whole front page so that the background, title and button comes up from underneath in a satisfying way **(In the gif it doesn't look as smooth as it has less FPS)**

-----------------------------

![e6cdb70deedcf15c1262f2be6e12468f](uploads/48ac41ecea61eca12bff0fe9ff8cdb60/e6cdb70deedcf15c1262f2be6e12468f.gif)

![2ca35d02ab556781a81707cb9249a238](uploads/54ccb55f423254a27cd2b068f04e233f/2ca35d02ab556781a81707cb9249a238.gif)

-----------------------------