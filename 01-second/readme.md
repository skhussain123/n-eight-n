n8n mein "Collector Node" koi khas ya official term nahi hai, lekin jab log iska zikr karte hain, toh woh aise nodes ki baat kar rahe hote hain jo data ko jama (collect) ya aggregate karte hain. n8n ek workflow automation tool hai jo mukhtalif nodes ke zariye data ko process, transform, aur transfer karta hai. Yeh kuch nodes hain jo "Collector Node" ke tor par kaam kar sakte


### Node arrows 
The arrows between nodes in an n8n workflow represent the flow of data or execution path—they show how output from one node feeds into subsequent nodes.
![""](./image.avif)<br>

#### What Do These Arrows Mean?

* Execution Flow: Arrows indicate the direction in which the workflow progresses. Once one node completes its task, arrows guide n8n to the next node in sequence.
* Data Passing: Each node processes input data (typically an array of JSON objects) and passes the transformed output to the next node through these connections 
* Branches & Merges: Arrows can split—so multiple nodes receive the same data—or converge, where different branches join back together.


### Why Are Workflows Inactive by Default?
As clarified in n8n’s documentation:<br>
“By default, all newly created workflows start deactivated.”
You need to manually activate them using the toggle at the top of the editor UI

#### Why This Behavior?
* Safety First: Automatically running new workflows could result in unexpected actions—like sending emails, making API calls, or altering data—without a chance to review them.
* Controlled Activation: It ensures you always consciously decide when a workflow should be allowed to run automatically.
