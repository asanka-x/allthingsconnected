---
layout: post
title: 4+1 View Model
date: 2013-03-31
tags: ["Tutorials"]
---

Architecture of software-intensive system can be described using multiple, concurrent views. Based on this fact [Philipe Kruchten](http://en.wikipedia.org/wiki/Philippe_Kruchten) developed a view model consists of 5 views, that a software architect can look at a system. But why is this called 4+1 view model rather 5 view model ? The obvious reason is unlike four views one view shows the systems functionality from the view point of the outside world.  
<div>  
</div><div>Following figure shows the 5 views, how they are related to each other and the diagrams used to explain each view.</div><div>  
</div><div class="separator" style="clear:both;text-align:center;">[![](http://asankanissanka.files.wordpress.com/2013/03/uml41.gif?w=300)](uml41.gif?w=300)</div><div>  
</div><div>**Logical View**</div><div>**  
**</div><div>

*   Shows the parts that&nbsp;compromise&nbsp;the systems
*   Represent a set of abstraction
*   Emphasizes classes and objects</div><div>  
</div><div>_<u>UML diagrams used</u>_</div><div>&nbsp; &nbsp; &nbsp; &nbsp; Class diagram  
&nbsp; &nbsp; &nbsp; &nbsp; State diagram  
&nbsp; &nbsp; &nbsp; &nbsp; Object diagram</div><div>  
</div><div>**Process View**</div><div>  
</div><div>

*   Describes system processes</div><div>_<u>UML diagrams used</u>_</div><div>&nbsp; &nbsp; &nbsp; &nbsp; Activity diagram</div><div>&nbsp; &nbsp; &nbsp; &nbsp; Sequence diagram</div><div>&nbsp; &nbsp; &nbsp; &nbsp; Communication diagram</div><div>  
</div><div>**Implementation View (Development&nbsp;View)**</div><div>**  
**</div><div>

*   Illustrates a system from a programmer's perspective</div><div>  
</div><div>_<u>UML diagrams used</u>_</div><div>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Component diagram</div><div>  
</div><div>**Deployment View (Physical View)**</div><div>**  
**</div><div>

*   Illustrates system execution environment
*   Maps software artifacts to hardware that hosts them</div><div>  
</div><div>_<u>UML diagrams used</u>_</div><div>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Deployment diagram</div><div>  
</div><div>**Use Case View**</div><div>**  
**</div><div>

*   Illustrates system functionality
*   Captures user goals and scenarios
*   Helpful in defining the structure and functionality in other 4 views</div><div>_<u>UML diagrams used</u>_</div><div>&nbsp; &nbsp; &nbsp; &nbsp; Use case diagram</div><div>**  
**</div><div></div><div>**  
**</div><div>**  
**</div><div>  
</div><div>  
</div>