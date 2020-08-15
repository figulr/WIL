# WIL
## What I Learned

2020.08.13.
## HTML vs. HTTP
*HTML<br>
a language for converting normal text into hypertext using tags like "<haed> ... </head>"<br>.
hypertext pages are interlinked as a part of the web.<br>
*HTTP<br>
a protocal for transferring HTML files (web pages) from web server to web browser using protocal mehtods like "GET, POST and so on".<br>

## XML
XML stans for eXtensible Markup Language (가확장성 마크업 언어).<br>
XML dose not do anything.<br>
XML is written like HTML using tags in order to store and transport data but these tags are not predefined like tags of HTML.<br>
XML does not work active but it is just self-descriptive.<br>
That XML is extensible means that XML helps to exchange data between incompatible systems without writing same data into severeal different forms. For it, XML is written in format of a plain text.<br>
## XML vs. HTML
XML for transporting data to focus on what data is.<br>
HTML for displaying data to focus on how data looks.<br>

*Reference
https://www.w3schools.com/<br>

## AJAX
AJAX stands for Asynchronous Javascript And XML.<br>
Using AJAX several types of data are exchanged for example JSON, XML, HTML, Text and so on.<br>
A strong positive thing is to exchange data without refreshing the already loaded web page, but updating only the required part. Thus it is called as asynchronous.<br>

*abstracted Example from MDN web docs
<pre><code>
<button id="ajax" type="button">Request</button>
<script>
function (){
  var httpRequest;
  documnet.getElementById("ajax").addEventListenre('click', makeRequest);
  
  function makeRequest(){
    httpRequest = new XMLHttpRequest();
    
    if(!httpRequest){
    alert("Cannot create XMLHTTP instance");
    return false;
    }
    httpRequest.onreadystatechange = alertContents;
    httpRequest.open('GET', 'test.html');
    httpRequest.send();
  }
  function alertContents(){
    if(httpRequest.readyState === XMLHttpRequest.DONE){
      if(httpRequest.status === 200){
        alert(httpRequest.responseText);
      } else{
        alert('A problem occurs in request);
      }
    }
  }
}
</script>
</code></pre>

*Reference
https://developer.mozilla.org/<br>


