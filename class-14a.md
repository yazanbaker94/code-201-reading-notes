#  What Google Learned About Teams


So Rozovsky started looking for other groups she could join. A classmate mentioned that some students were putting together teams for ‘‘case competitions,’’ contests in which participants proposed solutions to real-world business problems that were evaluated by judges, who awarded trophies and cash. The competitions were voluntary, but the work wasn’t all that different from what Rozovsky did with her study group: conducting lots of research and financial analyses, writing reports and giving presentations. The members of her case-competition team had a variety of professional experiences: Army officer, researcher at a think tank, director of a health-education nonprofit organization and consultant to a refugee program. Despite their disparate backgrounds, however, everyone clicked. They emailed one another dumb jokes and usually spent the first 10 minutes of each meeting chatting. When it came time to brainstorm, ‘‘we had lots of crazy ideas,’’ Rozovsky said.



It always struck Rozovsky as odd that her experiences with the two groups were dissimilar. Each was composed of people who were bright and outgoing. When she talked one on one with members of her study group, the exchanges were friendly and warm. It was only when they gathered as a team that things became fraught. By contrast, her case-competition team was always fun and easygoing. In some ways, the team’s members got along better as a group than as individual friends.



In Silicon Valley, software engineers are encouraged to work together, in part because studies show that groups tend to innovate faster, see mistakes more quickly and find better solutions to problems. Studies also show that people working in teams tend to achieve better results and report higher job satisfaction. In a 2015 study, executives said that profitability increases when workers are persuaded to collaborate more. Within companies and conglomerates, as well as in government agencies and schools, teams are now the fundamental unit of organization. If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.



As they struggled to figure out what made a team successful, Rozovsky and her colleagues kept coming across research by psychologists and sociologists that focused on what are known as ‘‘group norms.’’ Norms are the traditions, behavioral standards and unwritten rules that govern how we function when we gather: One team may come to a consensus that avoiding disagreement is more valuable than debate; another team might develop a culture that encourages vigorous arguments and spurns groupthink. Norms can be unspoken or openly acknowledged, but their influence is often profound. Team members may behave in certain ways as individuals — they may chafe against authority or prefer working independently — but when they gather, the group’s norms typically override individual proclivities and encourage deference to the team.


After looking at over a hundred groups for more than a year, Project Aristotle researchers concluded that understanding and influencing group norms were the keys to improving Google’s teams. But Rozovsky, now a lead researcher, needed to figure out which norms mattered most. Google’s research had identified dozens of behaviors that seemed important, except that sometimes the norms of one effective team contrasted sharply with those of another equally successful group. Was it better to let everyone speak as much as they wanted, or should strong leaders end meandering debates? Was it more effective for people to openly disagree with one another, or should conflicts be played down? The data didn’t offer clear verdicts. In fact, the data sometimes pointed in opposite directions. The only thing worse than not finding a pattern is finding too many of them



In 2008, a group of psychologists from Carnegie Mellon, M.I.T. and Union College began to try to answer a question very much like this one. ‘‘Over the past century, psychologists made considerable progress in defining and systematically measuring intelligence in individuals,’’ the researchers wrote in the journal Science in 2010. ‘‘We have used the statistical approach they developed for individual intelligence to systematically measure the intelligence of groups.’’ Put differently, the researchers wanted to know if there is a collective I. Q. that emerges within a team that is distinct from the smarts of any single member.

As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ On some teams, everyone spoke during each task; on others, leadership shifted among teammates from assignment to assignment. But in each case, by the end of the day, everyone had spoken roughly the same amount. ‘‘As long as everyone got a chance to talk, the team did well,’’ Woolley said. ‘‘But if only one person or a small group spoke all the time, the collective intelligence declined.’’



Within psychology, researchers sometimes colloquially refer to traits like ‘‘conversational turn-taking’’ and ‘‘average social sensitivity’’ as aspects of what’s known as psychological safety — a group culture that the Harvard Business School professor Amy Edmondson defines as a ‘‘shared belief held by members of a team that the team is safe for interpersonal risk-taking.’’ Psychological safety is ‘‘a sense of confidence that the team will not embarrass, reject or punish someone for speaking up,’’ Edmondson wrote in a study published in 1999. ‘‘It describes a team climate characterized by interpersonal trust and mutual respect in which people are comfortable being themselves.’’



For Project Aristotle, research on psychological safety pointed to particular norms that are vital to success. There were other behaviors that seemed important as well — like making sure teams had clear goals and creating a culture of dependability. But Google’s data indicated that psychological safety, more than anything else, was critical to making a team work.



After Rozovsky gave one presentation, a trim, athletic man named Matt Sakaguchi approached the Project Aristotle researchers. Sakaguchi had an unusual background for a Google employee. Twenty years earlier, he was a member of a SWAT team in Walnut Creek, Calif., but left to become an electronics salesman and eventually landed at Google as a midlevel manager, where he has overseen teams of engineers who respond when the company’s websites or servers go down.






After Sakaguchi spoke, another teammate stood and described some health issues of her own. Then another discussed a difficult breakup. Eventually, the team shifted its focus to the survey. They found it easier to speak honestly about the things that had been bothering them, their small frictions and everyday annoyances. They agreed to adopt some new norms: From now on, Sakaguchi would make an extra effort to let the team members know how their work fit into Google’s larger mission; they agreed to try harder to notice when someone on the team was feeling excluded or down.



### ‘As long as everyone got a chance to talk, the team did well. But if only one person or a small group spoke all the time, the collective intelligence declined.’


‘‘That could have been the wrong thing to say to someone else, but he knew it was exactly what I needed to hear,’’ Rozovsky said. ‘‘With one 30-second interaction, we defused the tension.’’ She wanted to be listened to. She wanted her teammate to be sensitive to what she was feeling. ‘‘And I had research telling me that it was O.K. to follow my gut,’’ she said. ‘‘So that’s what I did. The data helped me feel safe enough to do what I thought was right.’’




<hr>
<hr>
<hr>



Transform Syntax
The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.







          div {
            -webkit-transform: scale(1.5);
               -moz-transform: scale(1.5);
                 -o-transform: scale(1.5);
                    transform: scale(1.5);
          }




2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.




2D Rotate
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.




            <figure class="box-1">Box 1</figure>
            <figure class="box-2">Box 2</figure>



            .box-1 {
              transform: rotate(20deg);
            }
            .box-2 {
              transform: rotate(-55deg);
            }





2D Scale
Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.




        <figure class="box-1">Box 1</figure>
        <figure class="box-2">Box 2</figure>



        .box-1 {
          transform: scale(.75);
        }
        .box-2 {
          transform: scale(1.25);
        }




2D Translate
The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.





2D Skew
The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

The distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here.



Transform Origin
As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.

The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

Individually the values are treated like that of a background image position, using either a length or keyword value. That said, 0 0 is the same value as top left, and 100% 100% is the same value as bottom right. More specific values can also be set, for example 20px 50px would set the origin to 20 pixels across and 50 pixels down the element.




3D Scale
By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis, however the rotateX value is added in order to see the behavior of the scaleZ value. When removing the rotateX in this case, the elements will appear to be unchanged.



3D Translate
Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.

While this may appear to be very similar to that of the two-dimensional transform scale value, it is actually quite different. The transform is taking place on the z axis, not the x or y axes. When working with three-dimensional transforms, being able to move an element on the z axis does have great benefits, like when building the cube below for example.




Backface Visibility
When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.

The other value to backface-visibility is visible which is the default value, always displaying an element, no matter which direction it faces.

In the demonstration below notice how the second box isn’t displayed because backface-visibility: hidden; declaration has been set. The backface-visibility property takes even more significance when using animations.



Transitions
As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

In the example below the box will change its background color over the course of 1 second in a linear fashion.




        .box {
          background: #2db34a;
          transition-property: background;
          transition-duration: 1s;
          transition-timing-function: linear;
        }
        .box:hover {
          background: #ff7b29;
        }




Animations Keyframes
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.


          @keyframes slide {
            0% {
              left: 0;
              top: 0;
            }
            50% {
              left: 244px;
              top: 100px;
            }
            100% {
              left: 488px;
              top: 0;
            }
          }




Animation Duration, Timing Function, & Delay



        .stage:hover .ball {
          animation-name: slide;
          animation-duration: 2s;
        }



1. Fade in
Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:


          .fade
          {
                  opacity:0.5;
          }
          .fade:hover
          {
                  opacity:1;
          }



2. Change color
Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS:


        .color:hover
        {
                background:#53a7ea;
        }




3. Grow & Shrink
To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

Set your div’s class to “grow” and then add this code to your style block:


          .grow:hover
          {
                  -webkit-transform: scale(1.3);
                  -ms-transform: scale(1.3);
                  transform: scale(1.3);
          }




Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1:



          .shrink:hover
          {
                  -webkit-transform: scale(0.8);
                  -ms-transform: scale(0.8);
                  transform: scale(0.8);
          }




CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:



        .rotate:hover
        {
                -webkit-transform: rotateZ(-30deg);
                -ms-transform: rotateZ(-30deg);
                transform: rotateZ(-30deg);
        }



 5. Square to circle
A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

Give your div the class “circle” and add this CSS to your styles:


        .circle:hover
        {
                border-radius:50%;
        }



6. 3D shadow
3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

Give your div the class “threed” and then add the following code to your CSS:


          .threed:hover
          {
                  box-shadow:
                          1px 1px #53a7ea,
                          2px 2px #53a7ea,
                          3px 3px #53a7ea;
                  -webkit-transform: translateX(-3px);
                  transform: translateX(-3px);
          }



7. Swing
Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.


            @-webkit-keyframes swing
            {
                15%
                {
                    -webkit-transform: translateX(5px);
                    transform: translateX(5px);
                }
                30%
                {
                    -webkit-transform: translateX(-5px);
                   transform: translateX(-5px);
                } 
                50%
                {
                    -webkit-transform: translateX(3px);
                    transform: translateX(3px);
                }
                65%
                {
                    -webkit-transform: translateX(-3px);
                    transform: translateX(-3px);
                }
                80%
                {
                    -webkit-transform: translateX(2px);
                    transform: translateX(2px);
                }
                100%
                {
                    -webkit-transform: translateX(0);
                    transform: translateX(0);
                }
            }
            @keyframes swing
            {
                15%
                {
                    -webkit-transform: translateX(5px);
                    transform: translateX(5px);
                }
                30%
                {
                    -webkit-transform: translateX(-5px);
                    transform: translateX(-5px);
                }
                50%
                {
                    -webkit-transform: translateX(3px);
                    transform: translateX(3px);
                }
                65%
                {
                    -webkit-transform: translateX(-3px);
                    transform: translateX(-3px);
                }
                80%
                {
                    -webkit-transform: translateX(2px);
                    transform: translateX(2px);
                }
                100%
                {
                    -webkit-transform: translateX(0);
                    transform: translateX(0);
                }
            }






            .swing:hover
            {
                    -webkit-animation: swing 1s ease;
                    animation: swing 1s ease;
                    -webkit-animation-iteration-count: 1;
                    animation-iteration-count: 1;
            }






8. Inset border
One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

Give your div the class “border” and add the following CSS to your styles:





          .border:hover
          {
                  box-shadow: inset 0 0 0 25px #53a7ea;
          }






              
