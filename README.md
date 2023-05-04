Download Link: https://assignmentchef.com/product/solved-cs665-assignment-1-cache-covert-and-side-channel-attack
<br>
This programming assignment is designed to ensure that you are acquainted with the working principle of CPU Cache and its related security issues. In this assignment, you need to create a Cache Covert Channel to share information between Gogo and Gollu, running on two cores, in a multi-core system. Prior to create your covert channel, you can go through the <strong>“FLUSH+RELOAD” </strong>attack to get a feel and how to kick-start. The details about the attack is available in the web-link <a href="https://github.com/Anish-Saxena/Flush-Reload">https://github.com/ </a><a href="https://github.com/Anish-Saxena/Flush-Reload">Anish-Saxena/Flush-Reload</a><a href="https://github.com/Anish-Saxena/Flush-Reload">.</a> Once you understand the whats, hows, and whys, you are ready to go.

You can download/clone the code base and all other relevant files for PA1 from the following link <a href="https://github.com/skmtr1/CS665-2019-PA1">https://github.com/skmtr1/CS665-2019-PA1</a>

<h2>Part 1: Cache Covert Channel (FLUSH+RELOAD)</h2>

This part of the assignment deals with creating a covert channel between Gogo and Gollu that are running on two separate physical cores. They cannot communicate directly for confidentiality reasons and that’s why they need to create a covert channel to communicate so that no other processes could get the information. <strong>This part consist of two tasks:</strong>

<strong>Task 1a [It is Damn Easy !! 5 Points]: </strong>In this <strong>task</strong>, you need to create a <strong>Cache Covert Channel </strong>using <strong>FLUSH+RELOAD </strong>where <strong>Gogo </strong>reads some information from the terminal and sends it to the <strong>Gollu</strong>. You can assume that the information read from the terminal will not be of more than 50 characters. You have to report the covert channel bandwidth and the accuracy of the channel.

<strong>Task 1b [This is the real assignment !! 10 Points]: </strong>This Task is an extension to <strong>Task 1a</strong>. You need to share secret information but this time it will be a <strong>text </strong>file. You can choose any <strong>text </strong>file :). This task is further divided into the following subtasks:

<ol>

 <li><strong>Gogo </strong>first reads a filename from the terminal and communicate the filename to <strong>Gollu </strong>using the covert channel. You can assume that the file to be send will be in the current working directory of <strong>Gogo</strong>.</li>

 <li>After receiving the file name, <strong>Gollu </strong>creates a new blank file by appending <strong>received_ </strong>in front of the filename received from <strong>Gogo</strong>.</li>

</ol>

1

<ol start="3">

 <li>After sending the filename, <strong>Gogo </strong>then read the content of the file and communicate it to <strong>Gollu </strong>using covert channel again!</li>

 <li><strong>Gollu </strong>then writes all the received contents into a file that is earlier created by <strong>Gollu</strong>.</li>

 <li>You have to report the covert channel bandwidth and the accuracy of the channel.</li>

</ol>

[<strong>Note: </strong>Gogo and Gollu’s current working directories are different]

<h2>Cache Side Channel on GnuPG</h2>

<strong>Task 2a [easy peasy lemon squeezy, 5 Points]: </strong>In this task, you need to perform the <strong>FLUSH+RELOAD </strong>attack on <a href="https://gnupg.org/ftp/gcrypt/gnupg/gnupg-1.4.13.tar.gz">GnuPG</a> cryptography Library to observe accesses to critical functions like <strong>Square (S)</strong>, <strong>Module (r)</strong>, and <strong>Multiply (M) </strong>function during the encryption or decryption process of the RSA algorithm. For this assignment, <strong>Gogo </strong>will mount a side-channel attack with a goal to leak the critical accesses of <strong>Gollu</strong>. You have to report True Positive Rate and False Positive Rate of the side-channel.

<h2>If you want the Bonus points</h2>

<strong>Task 3a [Sounds interesting: Gogo and Gollu as Romeo and Juliet, 5 Points]: </strong>In this task, <strong>Gogo </strong>sends his heart (soul may be, in the form of an <strong>image </strong>file) to <strong>Gogo </strong>over the <strong>Cache Covert Channel</strong>, created using <strong>FLUSH+RELOAD </strong>attack. You have to report the covert channel bandwidth and the accuracy of the channel.

<strong>[Note: All the information sharing has to be performed through the Cache covert channel only.</strong>

<strong>All the task(s) has to be done on Linux Operating System. We will accept your submission via Canvas only, and any other submission mode is strictly prohibited such as submitting via email or piazza. While using Piazza/email for discussions, use CS665-PA1 as the header]</strong>