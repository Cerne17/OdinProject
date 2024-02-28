<h1 id="toc">Table of Contents</h1>
<ul>
    <li>
        <a href="#what-is-internet">What is the Internet</a>
    </li>
    <li>
        <a href="#packets">What are packets and their use in data transfer</a>
    </li>
    <li>
        <a href="#important-concepts">Important Concepts for Web</a>
    </li>
    <li>
        <a href="#how-the-web-works">How does the Web Work?</a>
    </li>
    <li>
        <a href="#links">Useful Links</a>
    </li>
</ul>
<hr>
<h2 id="what-is-internet">What is the Internet</h2>
<p>
    Is the connection between devices that enables communication through computers. Differently then many people believe, the world wide web and the internet aren't the same, the WWW uses the Internet to exist.
</p>
<h3 id="reference-link-table">Difference between Internet and Web</h3>
<p>
    The Internet is the barebones of the Web. It is, basically, the network of computers connected to each other.
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-2.png" alt="Internet with computers connected directly connected to each other" width="300px"/>
<p>
    This would be the internet if we needed to connect each computer to each other, it would be impossible!
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-3.png" alt="Internet with router" width="300px"/>
<p>
    To solve this issue, the idea of a router was created. It basically is an interface that receives all the connections and rerouts it to the right device.
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-4.png" alt="Internet with network of routers" width="300px"/>
<p>
    Even though the single router approach is much better then the 1:1 connections between computers, it still struggles with much more computers' networks. Thus, the system of multiple routers makes possible the infinite scalability of routers.
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-5.png" alt="Internet with network of routers" width="300px"/>
<p>
    Finally, to complete the Internet's schema, we need something to connect the independent devices to the network of routers. To accoomplish so, we use Modems. They are responsible for connecting our devices to the Internet, giving them the connection needed to reach other computers.
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work/internet-schema-7.png" alt="The complete Internet schema" width="300px"/>
<p>
    To connect the computers to the Internet, we need to follow the following schema: The local network is connected to an ISP (Internet Service Provider). The ISP companies are responsible for the connections of some specific routers, and they connect to the routers of other ISP companies, building up the Internet's complete network.
</p>
<h3 id="finding-computers">Reaching out Specific Computers</h3>
<p>
    To reach a specific computer in the network, you must identify which one you would like to contact. Thus, a kind of address is needed. In the computer area, this address is the IP (Internet Protocol). A IP address is a series of numbers spaced by dots. They are really difficult to remember, so when it comes to the Internet itself, developer created "nicknames" (aliases) for the sites, these aliases are called domains. A domain example could be: www.google.com; www.youtube.com; ...
</p>
<h3 id="internet-vs-web">Internet vs Web</h3>
<p>
    The Internet is the Infrastructure that makes it possible for people to create specific computers (Web Servers) that serve at the sites we know. This is what we call the Web. Thus, the Internet is the Infrastructure and the Web is the service built on top of this infrastructure.
</p>
<h3 class="extra-notes">Extra Notes</h3>
<ul>
    <li>
        <p>In the Internet, a router is found always two or more parts of the internet intersects.</p>
    </li>
</ul>
<hr>
<h2 id="packets">What are packets and why are they useful?</h2>
<p>
    Packets are small packs of data that are sent through the internet. The bigger traffics, such as videos, are split into smaller pieces - packets - to make it's way in the internet and travel through the internet.
</p>
<p>
    Packets are sent from your computer, and always they pass through a router and/or ISP, they get a wrapper, to state where they passed. Then, when the packet gets to the ending server, it takes off all the wrappers, discovering the massage within the packet itself. To send it back to your computer, it re-assembles the wrappings and always the packet get to the piece of internet that created a specific wrapper, it's taken off, to discover the next destination, until the packet make it's way back to your computer, with no wrappings.
</p>
<hr>
<h2 id="important-concepts">Webpage vs Website vs Webserver vs Search Engine</h2>
<p><b>Mozilla Definitions on these terms:</b></p>
<h3>web page</h3>
<p>
A document which can be displayed in a web browser such as Firefox, Google Chrome, Opera, Microsoft Edge, or Apple Safari. These are also often called just "pages."
</p>
<h3>website</h3>
<p>
A collection of web pages which are grouped together and usually connected together in various ways. Often called a "website" or a "site."
</p>
<h3>web server</h3>
<p>
A computer that hosts a website on the Internet.
</p>
<h3>search engine</h3>
<p>
A web service that helps you find other web pages, such as Google, Bing, Yahoo, or DuckDuckGo. Search engines are normally accessed through a web browser (e.g. you can perform search engine searches directly in the address bar of Firefox, Chrome, etc.) or through a web page (e.g. bing.com or duckduckgo.com).
</p>
<hr>
<h2 id="how-the-web-works">How does the Web Work?</h2>
<p>
    Computers in the web are usually called "Clients" and "Servers" and they change data with each other.
</p>
<img src="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works/simple-client-server.png" alt="Client and Server exchanging requests" height="200px"/>
<p>
    Clients: Normal internet users that want to access content online, commonly via a web browser in a PC.
</p>
<p>
    Servers: Computers that store webpages, websites and apps. When a client tries to access a webpage via their browser, they send a request to Servers, that sends back the information requested by the user.
</p>
<h3>Important Parts of The Web</h3>
<ol>
    <li>
        <p><b>Clients</b></p>
    </li>
    <li>
        <p><b>Servers</b></p>
    </li>
    <li>
        <p><b>Internet Connection</b></p>
    </li>
    <li>
        <p><b>TCP/IP: </b>(Transmission Control Protocol/ Internet Protocol) Protocols that dictate how the data can travel across the Internet</p>
    </li>
    <li>
        <p><b>DNS: </b>(Domain Name System) Basically the Addresses Book. When you type into your browser the webpage's Domain, the browser searches the DNS to find the respective IP address to that site before accessing it and retrieving it's data.</p>
    </li>
    <li>
        <p><b>HTTP: </b>(Hypertext Transfer Protocol) Application Protocol that enables the communication between the Clients and the Servers.</p>
    </li>
    <li>
        <p><b>Component Files:</b>The different files that compose a website. They can either be: code files or assets.</p>
    </li>
</ol>
<h3>Order the browser gets the Files</h3>
<ol>
    <li>
        Html file, in which the browser recognizes all the external links to stylesheets and script files.
    </li>
    <li>
        CSS and Javascript are then requested simultaneously.
    </li>
    <li>
        The browser then creates the DOM and CSSOM and, finally, renders the HTML, CSS and Javascript.
    </li>
</ol>
<h3>The Flow of requesting a webpage</h3>
<ol>
    <li>
        <p>
        The browser sends a request to the DNS request to get a the webpage's real address.
        </p>
    </li>
    <li>
        <p>
        The browser sends a HTTP request to the site trying to GET a copy of it's files to the Client, which is sent using the TCP/IP methods. 
        </p>
    </li>
    <li>
        <p>
        If the Server responds positively, it will respond with the code "200 OK" and retrieve all the data needed to assemble the webpage in packets. 
        </p>
    </li>
    <li>
        <p>
        Finally, the browser assembles the packets back into the webpage form and displays it at the user's screen.
        </p>
    </li>
</ol>
<hr>
<h2 id="links">Useful Links</h2>
<ul>
    <li>
        <a href="https://developer.mozilla.org/en-US/docs/Glossary" target="_blank">Web Development Glossary</a>
    </li>
    <li>
        <a href="https://www.youtube.com/watch?v=eHp1l73ztB8" target="_blank">What is the Internet?</a>
    </li>
    <li>
        <a href="https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/How_does_the_Internet_work" target="_blank">What is and how does the Internet work? (Mozilla)</a>
    </li>
    <li>
        <a href="https://www.youtube.com/watch?v=72snZctFFtA&t=45s" target="_blank">A DNS Request in action</a>
    </li>
</ul>
