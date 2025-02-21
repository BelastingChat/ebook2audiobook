📚 ebook2audiobook
CPU/GPU Converter from eBooks to audiobooks with chapters and metadata<br/>
सीपीयू/जीपीयू कनवर्टर ई -बुक्स से ऑडियोबुक तक अध्यायों और मेटाडेटा के साथ <br/>
कैलिबर, FFMPEG, XTTSV2, FAIRSEQ और अधिक का उपयोग करना। वॉयस क्लोनिंग और +1110 भाषाओं का समर्थन करता है! [!महत्वपूर्ण]
** यह उपकरण गैर-डीआरएम के साथ उपयोग के लिए है, कानूनी रूप से केवल अर्जित ई-बुक्स। ** <br>
लेखक इस सॉफ्टवेयर के किसी भी दुरुपयोग या किसी भी परिणामी कानूनी परिणामों के लिए जिम्मेदार नहीं हैं। <br>
इस उपकरण का उपयोग जिम्मेदारी से और सभी लागू कानूनों के अनुसार करें। ]

[![Discord](https://dcbadge.limes.pink/api/server/https://discord.gg/63Tv3F65k6)](https://discord.gg/63Tv3F65k6)

[! .com/Athomasson2)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/athomasson2) 


!
![demo_web_gui](assets/demo_web_gui.gif)

<details>
ara [العربية (अरबी)] (./ readme/readme_ar.md)
  <img width="1728" alt="GUI Screen 1" src="assets/gui_1.png">
  <img width="1728" alt="GUI Screen 2" src="assets/gui_2.png">
zho [中文 (चीनी)] (./ readme/readme_cn.md)
</details>


## README.md
- ara [العربية (Arabic)](./readme/README_AR.md)
Swe [Svenska (Swedish)]
- eng [English](README.md)
- swe [Svenska (Swedish)](./readme/README_SWE.md)
fas [رارسی (फ़ारसी)] (./ readme/readme_fa.md)


## Table of Contents
[ebook2audiobook] (#-ebook2audiobook)
- [Features](#features)
- [Docker GUI Interface](#docker-gui-interface)
[सुविधाएँ] (#विशेषताएं)
- [Free Google Colab](#free-google-colab)
- [Pre-made Audio Demos](#demos)
[डॉकर जीयूआई इंटरफ़ेस] (#डॉकर-गू-इंटेरफेस)
- [Requirements](#hardware-requirements)
- [Installation Instructions](#installation-instructions)
[हगिंगफेस स्पेस डेमो] (#हगिंग-स्पेस-डेमो)
  - [Launching Gradio Web Interface](#launching-gradio-web-interface)
  - [Basic Headless Usage](#basic--usage)
[मुफ्त Google Colab] (#फ्री-Google-Colab)
  - [Renting a GPU](#renting-a-gpu)
  - [Help command output](#help-command-output)
[पूर्व-निर्मित ऑडियो डेमो] (#डेमो)
  - [For Collection of Fine-Tuned TTS Models](#fine-tuned-tts-collection)
- [Using Docker](#using-docker)
[समर्थित भाषाएँ] (#समर्थित-भाषा)
  - [Docker Build](#building-the-docker-container)
  - [Docker Compose](#docker-compose)
[आवश्यकताएँ] (#हार्डवेयर-आवश्यकताएँ)
  - [Docker container file locations](#docker-container-file-locations)
  - [Common Docker issues](#common-docker-issues)
[स्थापना निर्देश] (#स्थापना-निर्देश)
- [Output](#output)
- [Common Issues](#common-issues)
[उपयोग] (#लॉन्चिंग-ग्रैडियो-वेब-इंटरफ़ेस)
- [Join Our  Server!](#join-our--server)
- [Legacy](#legacy-v10)
[लॉन्चिंग ग्रेडियो वेब इंटरफ़ेस] (#लॉन्चिंग-ग्रैडियो-वेब-इंटरफेस)


[बुनियादी हेडलेस उपयोग] (#मूल-उपयोग)
- 📖 Converts eBooks to text format with Calibre.
- 📚 Splits eBook into chapters for organized audio.
[हेडलेस कस्टम XTTS मॉडल उपयोग] (#उदाहरण-कस्टम-मॉडल-ज़िप-अपलोड)
- 🗣️ Optional voice cloning with your own voice file.
- 🌍 Supports +1110 languages (English by default). [List of Supported languages](https://dl.fbaipublicfiles.com/mms/tts/all-tts-languages.html)
[एक GPU किराए पर लेना] (#किराए पर लेना-A-GPU)


[मदद कमांड आउटपुट] (#सहायता-कमांड-आउटपुट)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Spaces-yellow?style=for-the-badge&logo=huggingface)](https://huggingface.co/spaces/drewThomasson/ebook2audiobook)
- Huggingface space is running on free cpu tier so expect very slow or timeout lol, just do not give it giant files is all
[ठीक ट्यून किए गए टीटीएस मॉडल] (#फाइन-ट्यून्ड-टीटीएस-मॉडल)


[फाइन-ट्यून्ड टीटीएस मॉडल के संग्रह के लिए] (#फाइन-ट्यून्ड-टीटीएस-संग्रह)
[![Free Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DrewThomasson/ebook2audiobook/blob/main/Notebooks/colab_ebook2audiobook.ipynb)


## Supported Languages
- **Arabic (ara)**
[डॉकर रन] (#रनिंग-द-डॉकर-कंटेनर)
- **Czech (ces)**
- **Croatian (hrv)**
[डॉकर बिल्ड] (#बिल्डिंग-द-डॉकर-कंटेनर)
- **English (eng)**
- **French (fra)**
[डॉकर कंपोज़] (#डॉकर-कम्पोज)
- **Hindi (hin)**
- **Hungarian (hun)**
[डॉकर हेडलेस गाइड] (#डॉकर-हेडलेस-गाइड)
- **Japanese (jpn)**
- **Korean (kor)**
[डॉकर कंटेनर फ़ाइल स्थान] (#डॉकर-कंटेनर-फाइल-लोकेशन)
- **Portuguese (por)**
- **Russian (rus)**
[कॉमन डॉकर मुद्दे] (#कॉमन-डॉकर-इश्यू)
- **Turkish (tur)**
- **Vietnamese (vie)**
[समर्थित ईबुक प्रारूप] (#समर्थित-ए-बुक-फॉर्मेट्स)


[आउटपुट] (#आउटपुट)
- 4gb RAM minimum, 8GB recommended
- Virtualization enabled if running on windows (Docker only)
[सामान्य मुद्दे] (#आम-मुद्दे)


[विशेष धन्यवाद] (#विशेष-धन्यवाद)
**Before to post an install or bug issue search carefully to the opened and closed issues TAB<br>
to be sure your issue does not exist already.**


>[!NOTE]
[विरासत] (#विरासत-वी 10)
you should first remove manually any text you don't want to be converted in audio.**


### Installation Instructions
विशेषताएँ
```bash
📖 कैलिबर के साथ पाठ प्रारूप में ई -बुक्स को परिवर्तित करता है। 📚 संगठित ऑडियो के लिए अध्यायों में ईबुक को विभाजित करता है। [Coqui XTTSV2] (https://huggingface.co/coqui/xtts-v2) और [FaireSeq] (https://github.com/facebookresearch/fairseq/tree/main/ के साथ उच्च गुणवत्ता वाले पाठ-टू-स्पीच उदाहरण/एमएमएस) (और अधिक)। 🗣 अपनी खुद की आवाज फ़ाइल के साथ वैकल्पिक आवाज क्लोनिंग। 🌍 +1110 भाषाओं (डिफ़ॉल्ट रूप से अंग्रेजी) का समर्थन करता है। [समर्थित भाषाओं की सूची] (https://dl.fbaipublicfiles.com/mms/tts/all-tts-languages.html)
```

🖥 4GB रैम पर चलने के लिए डिज़ाइन किया गया। [हगिंगफेस स्पेस डेमो] (https://huggingface.co/spaces/drewthomasson/ebook2audiobook)
1. **Run ebook2audiobook**:
[! /ebook2audiobook)
     ```bash
     ./ebook2audiobook.sh  # Run Launch script
हगिंगफेस स्पेस मुफ्त सीपीयू टियर पर चल रहा है, इसलिए बहुत धीमी या टाइमआउट लोल की उम्मीद है, बस यह मत दें कि यह विशाल फाइलें हैं
   - **Windows**
     ```bash
स्थान को डुप्लिकेट करने या स्थानीय रूप से चलाने के लिए सबसे अच्छा। नि: शुल्क Google Colab
     ```
] मुख्य/नोटबुक/colab_ebook2audiobook.ipynb)
3. **For Public Link**:
समर्थित भाषाएँ
   `./ebook2audiobook.sh --share` (Linux/MacOS)
** अरबी (आरा) **

> [!IMPORTANT]
** चीनी (zho) **
to let the web page reconnect to the new connection socket.**

** चेक (CES) **
   - **Linux/MacOS**:
     ```bash
** क्रोएशियाई (एचआरवी) **
         --voice [path_to_voice_file] --language [language_code]
     ```
** डच (एनएलडी) **
     ```bash
     .\ebook2audiobook.cmd --headless --ebook <path_to_ebook_file>
** अंग्रेजी (Eng) **
     ```
     
** फ्रेंच (फ्रा) **
  - **[--voice]**: Voice cloning file path (optional).
  - **[--language]**: Language code in ISO-639-3 (i.e.: ita for italian, eng for english, deu for german...).<br>
** जर्मन (Deu) **
    The ISO-639-1 2 letters codes are also supported.


###  Example of Custom Model Zip Upload
  (must be a .zip file containing the mandatory model files. Example for XTTS: config.json, model.pth, vocab.json and ref.wav)
** हंगेरियन (हुन) **
     ```bash
     ./ebook2audiobook.sh --headless --ebook <ebook_file_path> \
** इटैलियन (ITA) **
     ```
   - **Windows**
** जापानी (जेपीएन) **
     .\ebook2audiobook.cmd --headless --ebook <ebook_file_path> \
         --voice <target_voice_file_path> --language <language> --custom_model <custom_model_path>
** कोरियाई (कोर) **
- **<custom_model_path>**: Path to `model_name.zip` file,
      which must contain (according to the tts engine) all the mandatory files<br>
** पोलिश (पोल) **


** पुर्तगाली (पोर) **
   - **Linux/MacOS**
     ```bash
** रूसी (आरयूएस) **
     ```
   - **Windows**
** स्पेनिश (स्पा) **
     .\ebook2audiobook.cmd --help
     ```
** तुर्की (तूर) **
    ```python
     app.py --help
** वियतनामी (vie) **

<a id="help-command-output"></a>
[** +1100 भाषाओं के माध्यम से FairSeq **]
usage: app.py [-h] [--script_mode SCRIPT_MODE] [--session SESSION] [--share]
हार्डवेयर आवश्यकताएँ
              [--language LANGUAGE] [--voice VOICE] [--device {cpu,gpu,mps}]
4GB रैम न्यूनतम, 8GB की सिफारिश की
              [--custom_model CUSTOM_MODEL] [--fine_tuned FINE_TUNED]
              [--output_format OUTPUT_FORMAT] [--temperature TEMPERATURE]
Windows (केवल डॉकर) पर चलने पर वर्चुअलाइजेशन सक्षम
              [--repetition_penalty REPETITION_PENALTY] [--top_k TOP_K] [--top_p TOP_P]
              [--speed SPEED] [--enable_text_splitting] [--output_dir OUTPUT_DIR]
सीपीयू, जीपीयू (अनुशंसित), एमपीएस (अभी तक अनुकूलित नहीं है और सीपीयू की तुलना में धीमा हो सकता है) संगत

Convert eBooks to Audiobooks using a Text-to-Speech model. You can either launch the Gradio interface or run the script in headless mode for direct conversion.

** एक स्थापित या बग समस्या पोस्ट करने से पहले खुले और बंद मुद्दों को ध्यान से खोजें टैब <br>
यह सुनिश्चित करने के लिए कि आपका मुद्दा पहले से मौजूद नहीं है। **
  --session SESSION     Session to resume the conversion in case of interruption, crash, 
                            or reuse of custom models and custom cloning voices.

** किसी भी मानक संरचना की कमी जैसे कि एक अध्याय, पैराग्राफ, प्रस्तावना आदि <br>
आपको पहले मैन्युअल रूप से किसी भी पाठ को हटा देना चाहिए जिसे आप ऑडियो में परिवर्तित नहीं करना चाहते हैं। **

स्थापना निर्देश

** क्लोन रेपो **
  --headless            Run the script in headless mode
लॉन्चिंग ग्रेडियो वेब इंटरफ़ेस
  --ebooks_dir EBOOKS_DIR
** ebook2audiobook चलाएं **:
                            Cannot be used when --ebook is present.
  --language LANGUAGE   Language of the e-book. Default language is set 
** लिनक्स/मैकओएस **

optional parameters:
** विंडोज **
                            Uses the default voice if not present.
  --device {cpu,gpu,mps}
** वेब ऐप खोलें ** सार्वजनिक लिंक के लिए **:
`पायथन app.py - -शार्ड` (सभी ओएस)
`।
`ebook2audiobook.cmd - -Share` (Windows)
                            Default depends on the selected language. The tts engine should be compatible with the chosen language
  --custom_model CUSTOM_MODEL
[!महत्वपूर्ण]
** यदि स्क्रिप्ट को रोक दिया जाता है और फिर से चलाया जाता है, तो आपको अपने ग्रैडियो GUI इंटरफ़ेस <br> को ताज़ा करने की आवश्यकता है
वेब पेज को नए कनेक्शन सॉकेट को फिर से जोड़ने दें। **
                        (Optional) Fine tuned model path. Default is builtin model.
मूल उपयोग
                        (Optional) Output audio format. Default is set in ./lib/conf.py
** लिनक्स/मैकओएस **:
                        (xtts only, optional) Temperature for the model. 
                            Default to config.json model. Higher temperatures lead to more creative outputs.
** विंडोज **
                        (xtts only, optional) A length penalty applied to the autoregressive decoder. 
                            Default to config.json model. Not applied to custom models.
** [-ईबुक] **: अपनी ईबुक फ़ाइल का पथ। ** [-आवाज] **: वॉयस क्लोनिंग फ़ाइल पथ (वैकल्पिक)। ** [-भाषा] **: आईएसओ -639-3 में भाषा कोड (यानी: इटालियन के लिए आईटीए, अंग्रेजी के लिए इंग्लिश, जर्मन के लिए डीयू ...)। <br>
डिफ़ॉल्ट भाषा ENG और -भाषा में डिफ़ॉल्ट भाषा सेट के लिए वैकल्पिक है ।/lib/lang.py। <br>
ISO-639-1 2 अक्षर कोड भी समर्थित हैं। कस्टम मॉडल ज़िप अपलोड का उदाहरण
  --repetition_penalty REPETITION_PENALTY
।
                            Default to config.json model.
  --top_k TOP_K         (xtts only, optional) Top-k sampling. 
** लिनक्स/मैकओएस **
                            Default to config.json model.
  --top_p TOP_P         (xtts only, optional) Top-p sampling. 
** विंडोज **
  --speed SPEED         (xtts only, optional) Speed factor for the speech generation. 
                            Default to config.json model.
"
    जिसमें शामिल होना चाहिए (टीटीएस इंजन के अनुसार) सभी अनिवार्य फाइलें <br>
    (देखें ./lib/models.py)। उपयोग करने के लिए सभी मापदंडों की सूची के साथ विस्तृत गाइड के लिए
  --output_dir OUTPUT_DIR
** लिनक्स/मैकओएस **
  --version             Show the version of the script and exit

** विंडोज **
Windows:
    Gradio/GUI:
** या सभी ओएस के लिए **
    Headless mode:
    ebook2audiobook.cmd --headless --ebook '/path/to/file'
<a id = "हेल्प-कमांड-आउटपुट"> </a>
    Gradio/GUI:
    ./ebook2audiobook.sh
नोट: Gradio/GUI मोड में, रनिंग रूपांतरण को रद्द करने के लिए, बस Ebook अपलोड घटक से [X] पर क्लिक करें। डॉकर का उपयोग करना
    ./ebook2audiobook.sh --headless --ebook '/path/to/file'
आप ईबुक को ऑडियोबुक कनवर्टर को चलाने के लिए डॉकर का उपयोग भी कर सकते हैं। यह विधि विभिन्न वातावरणों में स्थिरता सुनिश्चित करती है और सेटअप को सरल करती है। डॉकर कंटेनर चलाना

डॉकर कंटेनर को चलाने और ग्रेडियो इंटरफ़ेस शुरू करने के लिए, निम्न कमांड का उपयोग करें:

### Using Docker
-पू के साथ ही
This method ensures consistency across different environments and simplifies setup.


#### Running the Docker Container
डॉकर कंटेनर का निर्माण

आप कमांड के साथ डॉकर छवि बना सकते हैं:
```powershell
docker run --rm -p 7860:7860 athomasson2/ebook2audiobook
यह कमांड पोर्ट 7860 पर ग्रैडियो इंटरफ़ेस शुरू करेगा। (लोकलहोस्ट: 7860)
 -Run with GPU Speedup (NVIDIA compatible only)
```powershell
अधिक विकल्पों के लिए पैरामीटर `-help` जोड़ें
```


सभी ebook2audiobooks में `/होम/उपयोगकर्ता/ऐप/` का आधार dir होगा
उदाहरण के लिए:
`tmp` =`/घर/उपयोगकर्ता/ऐप/tmp`
`ऑडीओबूक्स` =`/होम/यूजर/ऐप/ऑडीओबूक्स`
```
डॉकर हेडलेस गाइड
- For more options add the parameter `--help`


## Docker container file locations
इससे पहले कि आप इसे चलाएं
जिसे लिंक किया जाएगा, यह वह जगह है जहाँ आप अपनी इनपुट फ़ाइलों को देखने के लिए डॉकर छवि के लिए रख सकते हैं
`tmp` = `/home/user/app/tmp`
`audiobooks` = `/home/user/app/audiobooks`


## Docker headless guide
और यह होना चाहिए! आउटपुट ऑडियोबुक को ऑडियोबुक फ़ोल्डर में मिलेगा जो भी स्थित होगा
अपने स्थानीय dir में आपने इस डॉकर कमांड को चलाया
docker pull athomasson2/ebook2audiobook
अन्य मापदंडों के लिए सहायता कमांड प्राप्त करने के लिए यह कार्यक्रम आप इसे चला सकते हैं
- Before you do run this you need to create a dir named "input-folder" in your current dir
और यह आउटपुट होगा 
[मदद कमांड आउटपुट] (#सहायता-कमांड-आउटपुट)
mkdir input-folder && mkdir Audiobooks
डॉकर रचना
- In the command below swap out **YOUR_INPUT_FILE.TXT** with the name of your input file 
यह परियोजना स्थानीय रूप से चलाने के लिए डॉकर की रचना का उपयोग करती है। आप GPU समर्थन को सक्षम या अक्षम कर सकते हैं 
या तो `*gpu- सक्षम` या`*gpu-disabled` `docker-compose.yml` सेट करके सेट करके
    -v $(pwd)/input-folder:/home/user/app/input_folder \
दौड़ने के लिए कदम
    athomasson2/ebook2audiobook \
** रिपॉजिटरी को क्लोन करें ** (यदि आप पहले से ही नहीं हैं):
```
- And that should be it! 
** GPU समर्थन सेट करें (डिफ़ॉल्ट रूप से अक्षम) **
GPU समर्थन को सक्षम करने के लिए, `docker-compose.yml` को संशोधित करें और`*GPU-DISABLED` को `*GPU- सक्षम` में बदलें


** सेवा शुरू करें: **

```bash
** सेवा का उपयोग करें: **

```
!
[Help command output](#help-command-output)


इसे चलाने के लिए हार्डवेयर नहीं है या आप एक GPU किराए पर लेना चाहते हैं? आप ह्यूगिनफेस स्पेस को डुप्लिकेट कर सकते हैं और लगभग $ 0.40 प्रति घंटे के लिए एक GPU किराए पर ले सकते हैं
This project uses Docker Compose to run locally. You can enable or disable GPU support 
[हगिंगफेस स्पेस डेमो] (#हगिंग-स्पेस-डेमो)


[मुफ्त Google Colab] (#फ्री-Google-Colab)
1. **Clone the Repository** (if you haven't already):
सामान्य डॉकर मुद्दे
   git clone https://github.com/DrewThomasson/ebook2audiobook.git
Docker ठीक ट्यून किए गए मॉडल डाउनलोड करने के लिए अटक जाता है। (यह हर कंप्यूटर के लिए नहीं होता है, लेकिन कुछ इस मुद्दे पर चलते हैं)
प्रगति बार को अक्षम करना समस्या को ठीक करने के लिए प्रकट होता है,
जैसा कि चर्चा की गई थी [यहाँ #191 में] (https://github.com/drewthomasson/ebook2audiobook/issues/191)
इस फिक्स को `डॉकर रन` कमांड में जोड़ने का उदाहरण
3. **Start the service:**
ठीक ट्यून टीटीएस मॉडल
    docker-compose up -d
आप इस रेपो के साथ आसानी से अपने स्वयं के XTTs मॉडल को ठीक कर सकते हैं
]
  The service will be available at http://localhost:7860.


]
![demo_web_gui](assets/demo_web_gui.gif)

एक स्थान जिसे आप प्रशिक्षण डेटा को भी आसानी से डी-नोज़ करने के लिए उपयोग कर सकते हैं
]
  <img width="1728" alt="GUI Screen 1" src="assets/gui_1.png">
ठीक ट्यून टीटीएस संग्रह
  <img width="1728" alt="GUI Screen 3" src="assets/gui_3.png">
पहले से ही ठीक ट्यून किए गए टीटीएस मॉडल के हमारे संग्रह को खोजने के लिए,


## Renting a GPU
क़ौम
#### You can duplicate the hugginface space and rent a gpu for around $0.40 an hour
** बरसात दिन की आवाज **

#### Or you can try using the google colab for free!
(Be aware it will time out after a bit of your not messing with the google colab)
** डेविड एटनबोरो आवाज **


समर्थित ईबुक प्रारूप
- Docker gets stuck downloading Fine-Tuned models.
`
।
`.snb`,` .cbc`, `.rb`,` .tcr`
  Example of adding this fix in the `docker run` command
```Dockerfile
** सबसे अच्छा परिणाम **: `.epub` या` .mobi` स्वचालित अध्याय का पता लगाने के लिए
    -p 7860:7860 athomasson2/ebook2audiobook
उत्पादन


!
You can fine-tune your own xtts model easily with this repo
सामान्य मुद्दे:

CPU धीमा है (सर्वर SMP CPU पर बेहतर है) जबकि NVIDIA GPU में लगभग वास्तविक समय रूपांतरण हो सकता है। [इस बारे में चर्चा] (https://github.com/drewthomasson/ebook2audiobook/discussions/19#discussioncomment-10879846)
तेजी से बहुभाषी पीढ़ी के लिए मैं अपने अन्य सुझाव दूंगा

(हालांकि इसमें शून्य-शॉट वॉयस क्लोनिंग नहीं है, और सिरी गुणवत्ता की आवाज है, लेकिन यह सीपीयू पर बहुत तेज है)। "मुझे निर्भरता के मुद्दे हैं" - बस डॉकर का उपयोग करें, इसकी पूरी तरह से निहित है और एक हेडलेस मोड है,
 अधिक जानकारी के लिए डॉकर रन कमांड के अंत में `--हेल्प` पैरामीटर जोड़ें। "Im एक काटे गए ऑडियो मुद्दा हो रहा है!" - कृपया इसका एक मुद्दा बनाएं,

### Fine Tuned TTS Collection
मुझे क्या मदद चाहिए! 🙌
[चीजों की पूरी सूची यहां पाई जा सकती है] (https://github.com/drewthomasson/ebook2audiobook/issues/32)
For an XTTS custom model a ref audio clip of the voice reference is mandatory:


## Demos
संभावित रूप से कई भाषाओं के लिए रीडमे गाइड बनाना (केवल एक ही भाषा जो मुझे पता है वह अंग्रेजी है)
https://github.com/user-attachments/assets/d25034d9-c77f-43a9-8f14-0d167172b080


** COQUI TTS **: [Coqui tts github] (https://github.com/idiap/coquii-ai-tts)
https://github.com/user-attachments/assets/0d437a41-0b0d-48ed-8c9b-02763d5e48ea


## Supported eBook Formats
- `.epub`, `.pdf`, `.mobi`, `.txt`, `.html`, `.rtf`, `.chm`, `.lit`,
** ffmpeg **: [ffmpeg वेबसाइट] (https://ffmpeg.org)
  `.snb`, `.cbc`, `.rb`, `.tcr`
- **Best results**: `.epub` or `.mobi` for automatic chapter detection


[विरासत v1.0] (विरासत/v1.0)
- Creates a `['m4b', 'm4a', 'mp4', 'webm', 'mov', 'mp3', 'flac', 'wav', 'ogg', 'aac']` (set in ./lib/conf.py) file with metadata and chapters.
आप कोड [यहाँ] (विरासत/v1.0) देख सकते हैं। हमारे सर्वर में शामिल हों! ]