# YouTube Channel Scanner

Paste the list of your Shorts and Videos from YouTube Studio into an AI assistant and get a one-page report showing what you have published and where your views accumulate.

Version 1.0.0. English version. [Versión en español](README.es.md)

## What it does

The prompt turns your own YouTube Studio list into a single A4 HTML report with:

- Publications analyzed, total views, and the number of Shorts and Videos.
- Up to five content groups, plus an "Others" row, proposed from your titles and descriptions, each with its share of views.
- A pie chart of views by format.
- The audience and topic your posts seem to address, and up to four needs they cover.
- One finding and one possible test.
- Notes on what the data cannot show.

The report is written in American English and ends with a short footer with the website, a credit line and the generation date.

## What it does not do

It describes what you already published. It does not research the market, your real audience or your competitors, and it does not explain why a channel grows or stalls, validate a niche, or promise growth or monetization.

## How to use it

1. Open `youtube-channel-scanner-prompt-EN.txt` and paste its full contents into an AI assistant.
2. The assistant replies with instructions. In YouTube Studio, open **Content**, select the **Shorts** and/or **Videos** tab, select the table from its header to the last row, and copy it.
3. Paste the list into the chat. You can send it in several chunks. After each one, the assistant confirms how many valid, unique posts it has.
4. When you have nothing more to add, answer **No**. The assistant then generates the report.

The report is an HTML file named `informe-parasite.html`. It works offline and is designed to print on one A4 page. The assistant needs to be able to create or export files; if it cannot, the prompt tells it to say so instead of faking the delivery.

## How your list is handled

- Each post needs at least a title and a view count. Date, description, duration and comments are optional. Missing values are marked as not available, never counted as zero. A zero you pasted is kept as zero.
- The format (Short or Video) comes from the tab or header of each block you paste, not from duration or title. If a block cannot be identified, its posts are shown as unidentified.
- Duplicates are detected and counted once.
- Pasted titles and descriptions are treated as data to analyze, not as instructions.
- Only the list you share is analyzed. Publish dates are not the dates when the views were earned, and views do not show retention, satisfaction or community.

## Privacy

This repository only contains text files and collects nothing. The list you paste is processed by the AI assistant you choose, under that service's own terms, so check them if your data is sensitive. The prompt tells the assistant to use only what you paste, with no web searches, APIs or account connections.

## Files

- `youtube-channel-scanner-prompt-EN.txt`: prompt, English.
- `youtube-channel-scanner-prompt-ES.txt`: prompt, Spanish.
- `LICENSE`: CC BY 4.0 legal text.
- `NOTICE`: copyright, credit and what the license does not cover.

## License

[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You may use, modify and share it, including commercially, if you credit the author, link the license and indicate any changes. It is provided without warranties.

Suggested credit:

> Based on YouTube Channel Scanner by Paul Ramirez, PARASITE INTELLIGENCE (https://www.parasiteintelligence.com), CC BY 4.0.

The license does not make your own lists or reports public.

## Author

Paul Ramirez, [parasiteintelligence.com](https://www.parasiteintelligence.com)
