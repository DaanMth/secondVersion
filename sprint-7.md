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

Another part I wanted to add was the configuration inside a component, as I didn't have lots of time left I decided to make this non-functional. As I still needed to spend some time on the portfolio and user tests I decided that this wasn't the most important part and with the little time I gave myself I could make it non-functional. So I made it possible to open the + button underneath the components inside the board, which opens a configuration modal. In here you can choose which configuration you want, the choices being; DutyCalls, Mail or logging. When you choose one of the three and press save the blue button turns red with a check mark giving the feedback that you have configured the component.

-----------------------------

![355a557366e12895f1ec7e73f0f4419b](uploads/bb399467bb541c7fd862c4f86ebc21f9/355a557366e12895f1ec7e73f0f4419b.gif)

## Navigating through the board

The last functionality that the stakeholders really would love to see was a way to navigate through the board when it would become too big to view on your screen. For this I made a research document designing different ways to make this functionality work and doing research on which one of these could work the best. I chose to do this research first as I wanted to know what the users would like the most on the application as it is most important to know what your users want. I had a vision in mind already which I often have but seeing other peoples perspectives was a really good way to know how it can look as well. You can read the research document [here](uploads/9c740cb65dc031492e0d400956d480f4/Navigate_Research.pdf)
Inside the research document you can try out the different designs that I made in Figma, it is linked to the specific page where you can try it out. This research really helped giving me guidance on what kind of way I want to navigate through the board, and it gave me a lot of different additional ideas from other perspectives. This really helped a lot and I'm happy with the results that I've got.


## Retrospective 
Before I had a retrospective with my stakeholders I first had a chat with Erik, I showed all the things that I have made with the given reason why I made certain choices. When I had shown everything we started focussing on what we should be doing the next sprint. As I didn't have much time left Erik told me that I should be focussing on user testing the application, as this could bring some errors or bugs and you can also know why users make certain choices inside of the application. He also told me that I should be focussing on my portfolio and that he wanted to give some feedback in the upcoming sprint as well. I agreed with this and set this as my goal for the upcoming sprint.
After giving my retrospective to my stakeholders they also agreed with Erik that I should be focussing on my portfolio and that I should also be doing some tests inside of the application so that I can show that the code is clean and robust. They also wanted to have my portfolio, code and figma designs so that they could give me feedback after the holidays. So for the upcoming sprint I will be working on my portfolio and a lot of testing.