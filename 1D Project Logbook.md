# 1D Project Logbook

Done by: Tiang Pei Yuan 1003323
<!-- TOC -->
- [ Phase 1 (Week 1-4) ](#p1)
  - [ (22nd Sep) First Meeting: ](#22sep)
  - [ (24th Sep) Second Meeting: ](#24sep)
  - [ (16th Oct) Lab Checkoff: ](#16oct)
- [ Phase 2: Start of Electronic Game Design ](#p2)
  - [ (18th Oct) Meeting: ](#18oct)
  - [ (21st Oct) Consultation session: ](#21oct)
  - [ (4th Nov) Checkoff 1: ](#4nov)
  - [ (1st Dec) Reflections:](#1dec)
  - [ (4th Dec) Progress update:](#4dec)
  - [ (6th Dec) Exhibition:](#6dec)
  

<!-- /TOC -->

<a name="p1"></a>
## Phase 1 (Week 1-4)
<a name="22sep"></a>
### (22nd Sep) First Meeting:

Agenda: 

- Complete the full bit-adder
- Get to know the groupmates

What happened: We met at ARMS lab to get the soldering done since we still didn't had access to Digital System Lab. We first prototyped using the breadboard and completed the full bit adder circuit perfectly so we started soldering it to the PCB. We also borrowed a Dremel tool from my dear friends from EPD at the ARMS lab to cut the connection on the PCB between the chips and some parts of the circuit. Everything was going great until the soldering was all completed and when we tested it nothing worked. It felt like the logic was wrong but after staring at it for half an hour we still couldn't figure out what was wrong. Thus we ended the meeting and met up again on the 24th in Meeting 1b. 

Personally, in my team which consists of Yuxuan, Wang Wei and Luying, I only knew Yuxuan personally and thus I had to take this opportunity to know the rest of the team. I didn't have a very good impression of Wang Wei (sorry if you're reading this) at first because I noticed sometimes he doesn't come to class or comes late, but I have no idea who Luying was because we were in different classes. Now, (this was written on 18th Oct) I feel like they're all nice people who are willing to work together to make this work, although Luying is still a bit on the quiet side.
<a name="24sep"></a>
### (24th Sep) Second Meeting:

Agenda:

- Complete the full adder

What happened: So now we met up in the Digital System Labs and after re-soldering some of the circuit parts it still did not work, so we decided to re-solder just the IC chips. After re-soldering it then the full bit adder was completed and everything worked perfectly. So we thought we accidentally burnt the chip because we weren't provided the IC chip socket, but the **WEIRD** thing was that when we used the 'burnt' chips on a breadboard it worked perfectly fine?? So we just concluded our meeting as well and split up the work for the poster and the video. Also, we would individually look into the FPGA.

![photo_2019-09-24_20-48-13](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-09-24_20-48-13.jpg)
<a name="16oct"></a>
### (16th Oct) Lab Checkoff:

Agenda:

- Checkoff FPGA

LONG queue - Really messy as well, we queued up for a good 15 mins, then when we reached the counter the lab tech said 'this isn't a checkoff counter, go re-queue' and was frankly less than friendly. Then after we re-queued for 10 mins they opened the 2nd counter again and checked us off so it was really annoying. BUT good news is that Yuxuan managed to get the FPGA to work and the lab techs were really impressed by the speed and the neatness of the solution so I think all's well that ends well. 
<a name="p2"></a>
## Phase 2: Start of Electronic Game Design
<a name="18oct"></a>
### (18th Oct) Meeting:

Agenda: 

- Come up with ideas on how to tackle the problem

So we decided to meet up at the library in the morning to have more time to discuss. We came prepared with a few retro games that we individually researched on. We listed all the games out and thought about the good, the bad, and whether it is actually possible to implement the game on the MOJO given our limited knowledge. We also did some market research to find out what could assist us in building our games. Also, following Prof Oka's wisdom, we decided to have an array of games instead of just one in case that one couldn't work out. Hence, we narrowed our options to:

1) Minesweeper

2) A game that dodges obstacles (that may have random speed just to trigger people)

3) Flappy bird

4) Math game with windows that open/closes all the surrounding windows (one of the Math mod in Freshmore terms had that)

Also, we quickly booked a timeslot for consultation with Prof Nat so that we can order our parts earlier. Thus, the next meeting will be on 21st Oct.
<a name="21oct"></a>
### (21st Oct) Consultation session:

Agenda:

- Check off with Prof Natalie to ensure our ideas can work

We met at the tables outside CC13, and went through our ideas with Prof Nat. Generally I think it went well, Prof seems very pleased with the pre-research that we did, which was to source for materials as well as the idea. In the end we went with the idea of a 4x4 grid Minesweeper, and immediately after the consultation we gathered together to settle on the final purchases. By a stroke of luck, Yuxuan was actually planning to go back to China for recess week, so he is able to pick up the items much faster than waiting for the delivery.

![1572334819243](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/1572334819243.png)
<a name="4nov"></a>

### (4th Nov) Checkoff 1:

Agenda:

- Finish checkoff 1 

Due to a misunderstanding and miscommunication, we miraculously didn't do any work related to this checkoff at all during the recess week, as Yuxuan had went back to China and we mistakenly thought that the FPGA was with him, but it turns out that it was actually with Wang Wei. Thus, we met up on 4th Nov in the morning to gather at the Digital Systems Lab to do a sprint. The day started off quite badly as we aimed too high and wanted to use the seven-segment display to show the inputs and results of the ALU, so we had to write our own modules to convert to binary etc etc. Then, we realised that if we were to use the seven segment display we could only go up to 9999, which was a far cry from 16-bits, so we wasted half a day and we had to scrap that idea. In the end we went for the more typical, conventional way of displaying our results, which was to use the IO shield's LEDs. There were 3*8 = 24 LEDs, so 16 of them were used to display the 16 bits, and 3 were used to display 'z', 'v', and 'n'. We also used the dip switches to enter our 16 bits input, as well as the ALUFN signals for the OPCODE to indicate which operation we wanted. Thus, we ended up working till 3am in the morning but I am glad that we were able to finish it in time. Our physical checkoff is due on Thursday, 7th Nov and I hope nothing goes wrong.

<a name="1dec"></a>

### (1st Dec) Reflections:

Apologies for the lack of updates. After the checkoff previously, we did not score very well because we did not expect the auto testing mode and the manual testing mode to be so different from what we envisioned. Thus, we were quite disheartened but we had to pick ourselves up quickly to tackle the problem ahead, which was the actual game. During the checkoff of the report of the game with Prof Oka, it was well received and Prof complimented us that it was quite detailed and well done. Then, we split the work as such: I was in charge of the electronics and report, Yuxuan was in charge of the Mojo and the graphics, Luying was in charge of the graphics design and the Mojo, Wang Wei was in charge of the hardware and report. Personally, I spent about a total of 20 work hours in the Digital System Lab soldering our whole circuit together, which consisted of 16 RGB LEDs, 16 buttons as well as 16*5 female pin headers which we originally thought we could use, but they turned out to be unreliable.  
Before:

![photo_2019-11-27_17-56-11.jpg](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-11-27_17-56-11.jpg)

After:

![photo_2019-12-01_01-12-28.jpg](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-12-01_01-12-28.jpg)
![photo_2019-12-01_01-12-28 (2).jpg](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-12-01_01-12-28%20(2).jpg)

<a name="4dec"></a>

### (4th Dec) Progress update:

Wednesday of 1D week, 2 more days left to exhibition. Wang Wei was doing the hardware part and just last night Yuxuan submitted the poster as well as the Mojo code to EDimension, so currently I'm just working on the report because not everyone can work on the hardware together (which is actually pretty much settled already). 
![photo_2019-12-03_19-20-17.jpg](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-12-03_19-20-17.jpg)

<a name="6dec"></a>

### (6th Dec) Exhibition:

So on the exhibition day itself, I was at the booth the whole time and after explaining the game over a hundred times to different visitors, I feel like I became an expert in Minesweeper. However, the sad thing was that one of the LEDs blew on the morning itself, and we had no time to re-solder it, so I immediately changed the game rules while explaining for that tile to be a 'mystery tile', to increase the difficulty level because that tile will not tell you how many bombs is surrounding it. In general I think our game was quite well received and well liked, and we had quite a lot of votes from strangers that genuinely thought our game was fun. Especially the multiplayer aspect about it, which was very different and fresh from the normal typical minesweeper games. Overall, the response from the public kind of makes the effort and hard work we put in over the past term worth it.

![photo_2019-12-09_14-39-39.jpg](https://github.com/whenderpsfly/50.002_Logbook/blob/master/img/photo_2019-12-09_14-39-39.jpg)

