---
layout: post
title: "Add Network Printer in Windows"
thumbnail: add-printer-windows.png
tile-name: "Add Network Printer in Windows"
date: 2017-10-19

author: Media Center
tags: [media center]
---

## Windows 10

<br>
Click the `Start` menu and type in `Printers`. Select `Printers and Scanners`.

![Select Printers and Scanners](/img/add-printer-windows/01.png)<br>
_*Windows 7/8 is similar but use_ `Printer Settings` _from the_ `Control Panel`

<br>
Choose `Add a printer or scanner`
![Choose Add a printer or scanner](/img/add-printer-windows/02.png)

<br>
Do __NOT__ Select any printer from the list, even if you think you see the correct one this __will not work__.
Instead, after 5-15 seconds the option `The printer I want isn’t listed` will appear at the bottom of the list (you may need to scroll down slightly).
![The printer I want isn’t listed](/img/add-printer-windows/03.png)

<br>
On the next screen select `Add a printer using a TCP/IP address or hostname`
![Add a printer using a TCP/IP address or hostname](/img/add-printer-windows/04.png)

<br>
Select `TCP/IP Device` from the `Device type` menu, enter the IP Address of the Printer, and let Windows automatically fill in the `Port name`. Check the box to `Query the printer...` option as well. The IP addresses for SoA printers are listed at the bottom of this post.
![TCP/IP Device](/img/add-printer-windows/05.png)

<br>
If you are lucky, windows will detect the printer automatically. If not, you will need to select a driver, and perhaps even the networking device.

(Optional) This step is only required if you get the `Additional port information is required` dialogue box. If you do not receive this dialogue box, you can Skip to the next step. This dialogue means that you will need to select the networking type for the printer. For Ricoh select `Ricoh Generic Network`, for HP select `Hewlett Packard Jet Direct`. Dell has an option as well, and if you are unsure or do not see the choice you are looking for, “Generic Network Card” may also work. 
![Additional port information is required](/img/add-printer-windows/06.png)

<br>
(Optional) This step is only required if you get the `Install the printer driver` dialogue box. If you did not, you may proceed to the next step.
From this box you need to install a printer driver. Windows has many drivers built in, but not all. For Ricoh printers, you can select `RICOH` from the left pane, and `RICOH Class Driver` from the right. For HP or Dell you want to find the specific model of printer you are using. If you cannot find the appropriate driver, you may need to download it from the manufacturer’s website. If this is the case, you need to use the `Have Disk...` option and navigate to the driver folder once downloaded and extracted. Once you have the proper driver selected, click Next. 
![Install printer driver](/img/add-printer-windows/07.png)

<br>
Type in a name for the printer, this step is just for you and has no bearing on the printer. 

Select “Do Not Share This Printer”

Select Finish.

You have now installed a network Printer in Windows.

## SoA Printer IP Addresses

| Location                    | Model                     | IP Address      |
| -------------------         | -------------             | --------------- |
| CFA 213 Hallway &nbsp;&nbsp;| Ricoh 6430N &nbsp;&nbsp;  | `128.2.103.15`  |
| CFA 213 Hallway             | Dell 5330dn               | `128.2.103.126` |
| MMCH 309                    | Ricoh 6430N               | `128.2.108.209` |