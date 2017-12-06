# **Exploration 4**

** Objective: ** To find a web application developer job posting on glassdoor.com and research the requirements that have not been touched on in class.

**Career:**
* **Position:** Web Developer
* **Company:** Utah Retirement Systems located
* **Location:** Salt Lake City, UT
* **Links:**
  * Glassdoor: https://www.glassdoor.com/Job/jobs.htm?suggestCount=0&suggestChosen=false&clickSource=searchBtn&typedKeyword=web+developer&sc.keyword=web+developer&locT=&locId=&jobType=
  * Official Site: https://careers-urs.icims.com/jobs/2481/web-developer/job?mobile=false&needsRedirect=false


**Requirements:**
Must have a working knowledge of web authoring tools and languages such as:
* .NET framework  
* C#
* ASP.NET (4+)
* Linq
* SQL
* JQuery
* HTML
* XML
* JavaScript
* MS  MVC (3+)
* Razor

**What did I not know?**

After reading through the requirements, I realized that I am unfamiliar with:
* .NET framework  
* ASP.NET (4+)
* LINQ

And while I have heard of C#, I have never used it before. Therefore, I decided to play around with C# first.

** Background of unfamiliar language (links included): **

* **.NET framework:**
  * .NET Framework is a software framework developed by Microsoft that runs primarily on Microsoft Windows. It is an API with a main language being C#.
  * Link: https://en.wikipedia.org/wiki/.NET_Framework

* **ASP.NET:**
  * ASP.NET is an open source web framework for building modern web applications and services with .NET. ASP.NET creates websites based on HTML, CSS, and JavaScript.
  * Link: https://www.asp.net/
  * Note: https://www.asp.net/learn has a lot of games you can try to begin learning any of these languages listed.

* **LINQ:**
  * LINQ stands for Language Integrated Query. It is a Microsoft .NET Framework component that adds native data querying capabilities to .NET languages. LINQ extends the language (C#) by adding query expressions.
  * Link: https://en.wikipedia.org/wiki/Language_Integrated_Query

**Due to there being many languages that  are unfamiliar to me, I decided to dabble with C#, since that is the language it is mainly focused around.**


**Playing with C#**

I am very fortunate enough to have a friend that has programmed in C# before. He suggested that I download the Unity IDE (https://unity3d.com) and from there explore with game objects as well as learn C# (because coding isn't fun unless you get to play with weird objects).

After doing a couple of tutorials learning how Unity works, I developed a tiny program that allows you to move a cube back and forth on a plane. You are also allowed to change the colors of the cube (in my example only to green and red). Here is the code:

      using System.Collections;
      using System.Collections.Generic;
      using UnityEngine;

      public class NewBehaviourScript : MonoBehaviour {

      	// Use this for initialization
      	void Start () {

      	}

      	// Update is called once per frame
      	void Update () {
      		if (Input.GetKeyDown(KeyCode.C)){
      			gameObject.GetComponent<Renderer>().material.color = Color.red;
      		}

      		if (Input.GetKeyDown(KeyCode.R)){
      			//gameObject.GetComponent<Renderer>().material.color = Color.red;
      			gameObject.GetComponent<Rigidbody>().AddForce(2, 3, 0, ForceMode.Impulse);
      		}

      		if (Input.GetKeyDown(KeyCode.L)){
      			//gameObject.GetComponent<Renderer>().material.color = Color.red;
      			gameObject.GetComponent<Rigidbody>().AddForce(-2, 3, 0, ForceMode.Impulse);
      		}

      		if (Input.GetKeyDown(KeyCode.G)){
      			gameObject.GetComponent<Renderer>().material.color = Color.green;
      		}
      	}
      }

All this does is move a box left of right (L, R), and turns the box red of green (C, G). This is something a little more different than your typical "Hello World!" but it was nice to play around it.

**NOTE: Screenshots In Screenshots Folder**

**Conclusion:**

C# is a very powerful backend language that I wish I had more time to learn, and maybe with winter break coming up I might play around with Unity a little bit more! It's fascinating seeing what you can do with just one language.
