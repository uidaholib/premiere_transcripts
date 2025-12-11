---
title: Guide
nav: Guide
gallery: true
---

<br>

{% include feature/nav-menu.html sections="Open a New Project;Import Audio or Video Files;Configure Transcript Settings;Editing and Exporting Transcripts;Creating Captions" %}

<br>

{% include card.html text="Select any image embedded in this guide to expand" title="Note:" color="light" align="left" %}

<br>

## Open a New Project

<br>

- Open a `New Project` in Premiere

    {% include gallery-figure.html img="premiere_transcript_07.png" alt="Screenshot of Premiere interface start menu with the New Project button on the top left." width="100%" %}

- If it isn’t already set up by default, select the `Window` from the top menu and select `Text`, which should open on the top left of the interface

    {% include gallery-figure.html img="premiere_transcript_01.png" alt="Screenshot of Premiere with red arrows pointing to both the Window section of the top menu and the transcript window in the top left of the interface."  width="100%" %}

<br>

## Import Audio or Video Files

<br>

- Drop the audio from the media browser window on the bottom left into the timeline on the bottom left

    {% include gallery-figure.html img="premiere_transcript_08.png" alt="Screenshot of Premiere interface highlighting the media browser section."  width="100%" %}

- Drag that audio into the timeline section

    {% include gallery-figure.html img="premiere_transcript_06.png" alt="Screenshot of Premiere interface highlighting the timeline function."  width="100%" %}

<br>

## Configure Transcript Settings

<br>

- With the first `Transcript` tab open on the `Text` window, you will be given a prompt that says “do you want to auto transcribe media?” Instead, select the ellipses on the top right of the transcript window and then select `Generate Static Transcript`

    {% include gallery-figure.html img="premiere_transcript_03.png" alt="Screenshot of Premiere interface highlighting the transcript window and a red arrow pointing to the Generate Static Transcript function."  width="100%" %}

- This will open a window where you can specify the language of your media and whether you would like to differentiate speakers in your transcript. If you have only one speaker on a recording, confirming this will keep the platform from looking for other speakers.

    {% include gallery-figure.html img="premiere_transcript_02.png" alt="Screenshot of Premiere interface with Generate Static Transcript window."  width="100%" %}

- Depending on the length and language of the audio, processing should take between 5-15 minutes on a Mac device (longer on a PC)

- Once completed, you should have timestamps, generic speaker names (Speaker 1, Speaker 2, etc.) and dialogue

    {% include gallery-figure.html img="premiere_transcript_05.png" alt="Screenshot of CSV with transcript between two speakers, timestamps and dialogue." caption="Example of Premiere Transcript output in Google Sheets" width="100%" %}

<br>

## Editing and Exporting Transcripts

<br>

- While Adobe Sensei is one of the better transcription models we've tested, you will run into errors depending on the quality of the recording and the similarity of the speaker's voices

<br>

{% include alert.html text="One of the handy things about editing your transcripts in Premiere is that playback follows the text in the Transcript window, so it is a smoother workflow than coordinating with the audio player in one window and the transcript text in another" color="light" align="left" %}

<br>

- To edit the speaker names (which default to Speaker 1, Speaker 2, etc.) select the ellipses to the left of the dialogue, edit or add additional speakers

    {% include gallery-figure.html img="premiere_transcript_10.png" alt="Screenshot of the Premiere interface with red arrows pointing to the ellipses on the dialogue of the Transcript window, which opens the Edit Speakers module." width="100%" %}

- To edit the dialogue, simply double click whichever passage need configuring

    {% include gallery-figure.html img="premiere_transcript_09.png" alt="Screenshot of the Premiere interface with red arrows pointing a section of dialogue being edited." width="100%" %}

- While cleaning up dialogue is easy to do in Premiere, if you need to combine dialogue sections or create new fields, these will need to be done in a spreadsheet or document

- To export, click the ellipses on the `Text` window, find `Export` and choose either `CSV` for a spreadsheet or `TXT` for a document

    {% include gallery-figure.html img="premiere_transcript_04.png" alt="Screenshot of Premiere interface with highlight of transcript window and red arrow pointing to Export function." width="100%" %}

<br>

## Creating Captions

<br>

- First, select the `CC` Create Captions button in the `Transcript` window

    {% include gallery-figure.html img="premiere_transcript_11.png" alt="Screenshot of Premiere interface with an arrow pointing to the Create Captions button in the Transcript window." width="100%" %}

- This will open a `Create Captions` module that will have some options for formatting, spacing and how many lines you would like the captions to display as

    {% include gallery-figure.html img="premiere_transcript_12.png" alt="Screenshot of Premiere interface with an arrow pointing to the Create Captions button." width="100%" %}

- This will create a caption track, displayed above the video track on the timeline. To adjust the font, size and area that the captions will be displayed, select the entire track of dialogue in the timeline, then select `Window` from the top menu, then `Workspaces`, then `Captioning and Graphics`.

{% include gallery-figure.html img="premiere_transcript_13.png" alt="Screenshot of Premiere interface with an arrow pointing the new captions in the timeline as well as configurations in the Captions and Graphics window." width="100%" %}

- To add a translated caption, select the `Caption Translation` button, then configure the correct source language as well as what you would like the language to be translated to

{% include gallery-figure.html img="premiere_transcript_14.png" alt="Screenshot of Premiere interface with arrows pointing to the Caption Translation button and the various options you can configure this to." width="100%" %}

- Finally, adjust the positioning of the captions so they don't overlap. In this case, I have configured both caption tracks to display in two lines. By adjusting the `Set Vertical Position` of the Spanish language track to -60.00, this lifts the text up over the English language while still being generally oriented at the bottom of the display. Setting this to -30.00 should work if you chose to have captions generate in a single line display.

{% include gallery-figure.html img="premiere_transcript_15.png" alt="Screenshot of Premiere interface with arrows pointing at the selected caption track within the timeline and the Set Vertical Position function within the Captions and Graphics window." width="100%" %}

- To export these captions, select `Export` from the top left. Within this menu you can adjust your file name, export destination, and choose to export as a video, audio, gif or image file in the `Format` section (default will be mp4, which is a solid, lower file size option). When you have everything configured, select the `Export` function in the lower right hand corner.

{% include gallery-figure.html img="premiere_transcript_16.png" alt="Screenshot of Premiere interface with arrows pointing to the Export tab, Format and Export button." width="100%" %}

<br>

<div class="symbol-container">
    <p class="symbol">&#10042;</p>
</div>

<br>

<div style="width:100%; text-align:center;">

  <div role="img" aria-label="ASCII art of a lil’ transcript feller and a close captioned video reel feller — both smiling, celebrating how accessible they are." style="background-color:white; padding:20px; border-radius:12px; display:inline-block; text-align:center; box-shadow:0 2px 6px rgba(0,0,0,0.1);">

  <pre style="font-family: monospace; line-height: 1.1em; font-size: 14px; background-color:white; margin: 0 auto; display:inline-block; text-align:left;">
      ________                ╭──────╮
     /         \             /        \
    |           |           |   ╭──╮   |
    | TRANSCRIPT|          |    │CC│    |
    |   -----   |         |     ╰──╯     |
    |  ( •‿^ )  |         |   ( ^‿• )    |
    |   <   >   |          |    l  l    |
     \_________/             \  |  |  /
        /   \                 \______/
       /_____\               /   |   \
        |   |               /____|____\
       (b) (b)             (b)        (b)
  </pre>

  <p><b>That's it! Enjoy your accessible transcript file and/or captioned media!</b></p>

  </div>

</div>

<br>
