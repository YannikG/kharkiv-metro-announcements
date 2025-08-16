# Kharkiv Metro Announcements
**This repository contains a collection of Jupyter Notebooks to generate announcements for the Kharkiv metro system.**

## Background
I am a fan of public and rapid transportation, so in my recent trips to the fantastic city of Kharkiv in the eastern part of Ukraine. I kinda felt "in love" with the system and how it operates. Especially with the clear, calm and still informative automated announcements in the trains and in the stations. So I took some recordings of the original announcements and cloned it using AI (for private use only!) to recreate building blocks of the announcements.
 
## Disclaimer
The title is a bit misleading because this repository does not contain any audio files or mechanism to generate audio. I do not have any rights on the voice of the Kharkiv Metro, I am just a fan of the metro system and wanted to "preserve" the announcements in a way, so someone else can use the same steps to reproduce the (almost) real announcements of the Kharkiv metro.

# How to install
Before you start, make sure you have installed the required tooling.
## Requirements
- Python 3.8+
- Jupyter Notebook
- Audio processing tool FFmpeg [Download from Codec Guide](https://www.codecguide.com/download_kl.htm) or via Package Manager in Linux/Mac

## Install
1. Clone or download this repository
2. Create new virtual environment `python3 -m venv venv`
3. Activate virtual environment `./venv/Scripts/activate` or on Linux/Mac `source venv/bin/activate`
4. install dependencies using `pip install -r requirements.txt`
5. Open Jupyter Notebook and select the virtual environment as kernel

# How to recreate
To recreate the audio blocks, there are two possible ways:
## Quick and dirty with pre-defined Ukrainian voice
You can use any text to speech website or local model (that supports Ukrainian language) and use the table below to create the audio files.

## Original (like) voice
This is the method I used to generate my audio blocks.

1. Take some recordings of the announcements in a station or in the train. Make sure there is no other voice hearable and avoid any loud noises. Take several recordings with different pronunciation sounds. Stitch the recordings together to a +10 seconds audio file.
2. Use [Adobe Podcast AI enhance](https://podcast.adobe.com/en/enhance) to clean up the recording as much as possible.
3. Use an online voice cloning service to than clone the voice. For my audio blocks I used [ElevenLabs Text to Speech](https://elevenlabs.io/). Please note; make sure you have the rights to use the voice! **I am not responsible for ANY CONSEQUENCES**.
4. Use the table below to generate the audio blocks.

## Audio Blocks
> This list is currently not complete yet and does not include all the possible announcements! This list contains only the texts required to run the Jupyter Notebook without errors!

Other announcements are available here: https://gortransport.kharkov.ua/subway/sounds/

### Red Line (Холодногірсько-Заводська)
| Ukrainian Text                     | English Translation                     | File Path                                  |
|-------------------------------------|-----------------------------------------|--------------------------------------------|
| Станція Холодна Гора                | Kholodna Hora station                   | `stations/red_line/1_Холодна Гора.mp3`     |
| Станція Південний вокзал            | Pivdennyi Vokzal station                | `stations/red_line/2_Південний вокзал.mp3` |
| Станція Центральний ринок          | Tsentralnyi Rynok station               | `stations/red_line/3_Центральний ринок.mp3`|
| Станція Майдан Конституції         | Maidan Konstytutsii station             | `stations/red_line/4_Майдан Конституції.mp3`|
| Станція Левада                      | Levada station                          | `stations/red_line/5_Левада.mp3`           |
| Станція Спортивна                   | Sportyvna station                       | `stations/red_line/6_Спортивна.mp3`        |
| Станція Заводська                   | Zavodska station                        | `stations/red_line/7_Заводська.mp3`        |
| Станція Турбоатом                   | Turboatom station                       | `stations/red_line/8_Турбоатом.mp3`        |
| Станція Палац спорту                | Palats Sportu station                   | `stations/red_line/9_Палац спорту.mp3`     |
| Станція Армійська                   | Armiiska station                        | `stations/red_line/10_Армійська.mp3`       |
| Станція Масельського                | Maselskoho station                      | `stations/red_line/11-2_Масельськог.mp3`   |
| Станція Тракторний завод            | Traktornyi Zavod station                | `stations/red_line/12_Тракторний завод.mp3`|
| Станція Індустріальна               | Industrialna station                    | `stations/red_line/13_Індустріальна.mp3`  |

### Blue Line (Салтівська)
| Ukrainian Text                     | English Translation                     | File Path                                  |
|-------------------------------------|-----------------------------------------|--------------------------------------------|
| Станція Історичний музей           | Istorychnyi Muzei station               | `stations/blue_line/1_Історичний музей.mp3`|
| Станція Університет                 | Universytet station                     | `stations/blue_line/2_Університет.mp3`     |
| Станція Ярослава Мудрого            | Yaroslava Mudroho station               | `stations/blue_line/3_Ярослава Мудрого.mp3`|
| Станція Київська                    | Kyivska station                         | `stations/blue_line/4_Київська.mp3`        |
| Станція Академіка Барабашова       | Akademika Barabashova station           | `stations/blue_line/5_Академіка Барабашова.mp3`|
| Станція Академіка Павлова           | Akademika Pavlova station               | `stations/blue_line/6_Академіка Павлова.mp3`|
| Станція Студентська                 | Studentska station                      | `stations/blue_line/7_Студентська.mp3`     |
| Станція Салтівська                  | Saltivska station                       | `stations/blue_line/8_Салтівська.mp3`     |

### Green Line (Олексіївська)
| Ukrainian Text                     | English Translation                     | File Path                                  |
|-------------------------------------|-----------------------------------------|--------------------------------------------|
| Станція Перемога                    | Peremoha station                        | `stations/green_line/1_Перемога.mp3`       |
| Станція Олексіївська                | Oleksiivska station                     | `stations/green_line/2_Олексіївська.mp3`   |
| Станція 23 Серпня                   | 23 Serpnia station                      | `stations/green_line/3_23 Серпня.mp3`      |
| Станція Ботанічний Сад              | Botanichnyi Sad station                 | `stations/green_line/4_Ботанічний Сад.mp3` |
| Станція Наукова                     | Naukova station                         | `stations/green_line/5_Наукова.mp3`        |
| Станція Держпром                    | Derzhprom station                       | `stations/green_line/6_Держпром.mp3`       |
| Станція Архітектора Бекетова        | Arkhitektora Beketova station           | `stations/green_line/7_Архітектора Бекетова.mp3`|
| Станція Захисників України          | Zakhysnykiv Ukrainy station             | `stations/green_line/8_Захисників України.mp3`|
| Станція Метробудівників             | Metrobudivnykiv station                 | `stations/green_line/9_Метробудівників.mp3`|

### Transfer Announcements
| Ukrainian Text                                     | English Translation                     | File Path                                  |
|-----------------------------------------------------|-----------------------------------------|--------------------------------------------|
| Перехід на станцію Історичний музей до поїздів Салтівської лінії | Transfer to Istorychnyi Muzei station for Saltivska Line trains | `in_the_train/change_to/from_red_to_blue.mp3` |
| Перехід на станцію Майдан Конституції до поїздів Холодногірсько-Заводської лінії | Transfer to Maidan Konstytutsii station for Kholodnohirsko-Zavodska Line trains | `in_the_train/change_to/from_blue_to_red.mp3` |
| Перехід на станцію Метробудівників до поїздів Олексіївської лінії | Transfer to Metrobudivnykiv station for Oleksiivska Line trains | `in_the_train/change_to/from_red_to_green.mp3` |
| Перехід на станцію Спортивна до поїздів Холодногірсько-Заводської лінії | Transfer to Sportyvna station for Kholodnohirsko-Zavodska Line trains | `in_the_train/change_to/from_green_to_red.mp3` |
| Перехід на станцію Держпром до поїздів Олексіївської лінії | Transfer to Derzhprom station for Oleksiivska Line trains | `in_the_train/change_to/from_blue_to_green.mp3` |
| Перехід на станцію Університет до поїздів Салтівської лінії | Transfer to Universytet station for Saltivska Line trains | `in_the_train/change_to/from_green_to_blue.mp3` |

§

### In-Train Announcements
| Ukrainian Text                     | English Translation                     | File Path                                  |
|-------------------------------------|-----------------------------------------|--------------------------------------------|
| Наступна зупинка                    | Next stop                               | `in_the_train/next_stop.mp3`                |
| Обережно. двері зачиняються.        | Doors are closing                       | `in_the_train/doors_are_closing.mp3`        |
| Кінцева станція                     | Final stop                              | `in_the_train/final_stop.mp3`               |
| Будь ласка, не залишайте свої речі. | Please do not leave your belongings behind | `in_the_train/please_do_not_leave_your_belongings_behind_you.mp3` |
| Всього Вам найкращого!              | Good luck                               | `in_the_train/good_luck.mp3`                |

### Helpers
Create a about 1 second long silence audio file with the name `silence_between_stations.mp3` directly in the root audio folder.