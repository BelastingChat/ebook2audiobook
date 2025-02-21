# 📚 ebook2audiobook

CPU/GPU कनवर्टर eBooks से ऑडियोबुक तक अध्यायों और मेटाडेटा के साथ<br/>कैलिबर, FFMPEG, XTTSV2, FAIRSEQ और अधिक का उपयोग करना। वॉयस क्लोनिंग और +1110 भाषाओं का समर्थन करता है!

> [!महत्वपूर्ण]**यह उपकरण गैर-डीआरएम, कानूनी रूप से अधिग्रहित ई-बुक्स के साथ उपयोग के लिए है।**<br>लेखक इस सॉफ्टवेयर के किसी भी दुरुपयोग या किसी भी परिणामी कानूनी परिणामों के लिए जिम्मेदार नहीं हैं।<br>इस उपकरण का उपयोग जिम्मेदारी से और सभी लागू कानूनों के अनुसार करें।

[![Discord](https://dcbadge.limes.pink/api/server/https://discord.gg/63Tv3F65k6)](https://discord.gg/63Tv3F65k6)

Ebook2audiobook डेवलपर्स का समर्थन करने के लिए धन्यवाद!<br>[![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/athomasson2)

#### गुई इंटरफ़ेस

![demo_web_gui](assets/demo_web_gui.gif)

<details>
  <summary>Click to see images of Web GUI</summary>
  <img width="1728" alt="GUI Screen 1" src="assets/gui_1.png">
  <img width="1728" alt="GUI Screen 2" src="assets/gui_2.png">
  <img width="1728" alt="GUI Screen 3" src="assets/gui_3.png">
</details>

## README.md

-   हम ख़रीदते हैं[अरबी (अरबी)](./readme/README_AR.md)
-   ज़ो[चीनी](./readme/README_CN.md)
-   ए \`ए[अंग्रेज़ी](README.md)
-   swe [स्वीडिश (स्वीडिश)](./readme/README_SWE.md)
-   एफएएस[फारसी (फारसी)](./readme/README_FA.md)
-   वह[इतालवी (इतालवी)](./readme/README.it.md)

## विषयसूची

-   [ebook2audiobook](#-ebook2audiobook)
-   [विशेषताएँ](#features)
-   [डॉकर गुई इंटरफ़ेस](#docker-gui-interface)
-   [हगिंग स्पेस डेमो](#huggingface-space-demo)
-   [नि: शुल्क Google Colab](#free-google-colab)
-   [पूर्व-निर्मित ऑडियो डेमो](#demos)
-   [समर्थित भाषाएँ](#supported-languages)
-   [आवश्यकताएं](#hardware-requirements)
-   [स्थापना निर्देश](#installation-instructions)
-   [प्रयोग](#launching-gradio-web-interface)
    -   [लॉन्चिंग ग्रेडियो वेब इंटरफ़ेस](#launching-gradio-web-interface)
    -   [बुनियादी हेडलेस उपयोग](#basic--usage)
    -   [हेडलेस कस्टम XTTS मॉडल उपयोग](#example-of-custom-model-zip-upload)
    -   [एक GPU किराए पर लेना](#renting-a-gpu)
    -   [कमांड आउटपुट में मदद करें](#help-command-output)
-   [ठीक ट्यून टीटीएस मॉडल](#fine-tuned-tts-models)
    -   [फाइन-ट्यून किए गए टीटीएस मॉडल के संग्रह के लिए](#fine-tuned-tts-collection)
-   [डॉकर का उपयोग करना](#using-docker)
    -   [डॉकर रन](#running-the-docker-container)
    -   [डॉकर बिल्ड](#building-the-docker-container)
    -   [डॉकर रचना](#docker-compose)
    -   [डॉकर हेडलेस गाइड](#docker-headless-guide)
    -   [डॉकर कंटेनर फ़ाइल स्थान](#docker-container-file-locations)
    -   [सामान्य डॉकर मुद्दे](#common-docker-issues)
-   [समर्थित ईबुक प्रारूप](#supported-ebook-formats)
-   [उत्पादन](#output)
-   [सामान्य मुद्दे](#common-issues)
-   [विशेष धन्यवाद](#special-thanks)
-   [हमारे सर्वर में शामिल हों!](#join-our--server)
-   [परंपरा](#legacy-v10)
-   [विषयसूची](#table-of-contents)

## विशेषताएँ

-   📖 कैलिबर के साथ पाठ प्रारूप में ई -बुक्स को परिवर्तित करता है।
-   📚 संगठित ऑडियो के लिए अध्यायों में ईबुक को विभाजित करता है।
-   🎙 उच्च गुणवत्ता वाले पाठ-से-भाषण के साथ[Coqui XTTSV2](https://huggingface.co/coqui/XTTS-v2)और[फेयरसेक](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)(और अधिक)।
-   🗣 अपनी खुद की आवाज फ़ाइल के साथ वैकल्पिक आवाज क्लोनिंग।
-   🌍 +1110 भाषाओं (डिफ़ॉल्ट रूप से अंग्रेजी) का समर्थन करता है।[समर्थित भाषाओं की सूची](https://dl.fbaipublicfiles.com/mms/tts/all-tts-languages.html)
-   🖥️ Designed to run on 4GB RAM.

## [हगिंग स्पेस डेमो](https://huggingface.co/spaces/drewThomasson/ebook2audiobook)

[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Spaces-yellow?style=for-the-badge&logo=huggingface)](https://huggingface.co/spaces/drewThomasson/ebook2audiobook)

-   हगिंगफेस स्पेस मुफ्त सीपीयू टियर पर चल रहा है, इसलिए बहुत धीमी या टाइमआउट लोल की उम्मीद है, बस यह मत दें कि यह विशाल फाइलें हैं
-   स्थान को डुप्लिकेट करने या स्थानीय रूप से चलाने के लिए सबसे अच्छा।

## नि: शुल्क Google Colab

[![Free Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DrewThomasson/ebook2audiobook/blob/main/Notebooks/colab_ebook2audiobook.ipynb)

## समर्थित भाषाएँ

-   **अरबी**
-   **चीनी (ZH)**
-   **चेक (सीईएस)**
-   **क्रोएशियाई (एचआरवी)**
-   **डच (एनएलडी)**
-   **अंग्रेजी (Eng)**
-   **फ्रेंच (से)**
-   **जर्मन (DEU)**
-   **नहीं (हिन)**
-   **Hungarian (hun)**
-   **इटैलियन (आईटीए)**
-   **जापानी (जेपीएन)**
-   **कोरियाई (कोर)**
-   **पोलिश (पोल)**
-   **पुर्तगाली**
-   **रूसी (आरयूएस)**
-   **स्पेनिश (स्पा)**
-   **तुर्की (दौर)**
-   **वियतनामी (वीआईई)**
-   [**Fairseq के माध्यम से +1100 भाषाएँ**](https://dl.fbaipublicfiles.com/mms/tts/all-tts-languages.html)

## हार्डवेयर आवश्यकताएँ

-   4GB रैम न्यूनतम, 8GB की सिफारिश की
-   Windows (केवल डॉकर) पर चलने पर वर्चुअलाइजेशन सक्षम
-   सीपीयू, जीपीयू (अनुशंसित), एमपीएस (अभी तक अनुकूलित नहीं है और सीपीयू की तुलना में धीमा हो सकता है) संगत

> [!महत्वपूर्ण]**एक इंस्टॉल या बग समस्या पोस्ट करने से पहले खुले और बंद मुद्दों के टैब को सावधानी से खोजें<br>यह सुनिश्चित करने के लिए कि आपका मुद्दा पहले से मौजूद नहीं है।**

> [!टिप्पणी]**किसी भी मानक संरचना का अभाव जैसे कि एक अध्याय, पैराग्राफ, प्रस्तावना आदि।<br>आपको पहले मैन्युअल रूप से किसी भी पाठ को हटाना चाहिए जिसे आप ऑडियो में परिवर्तित नहीं करना चाहते हैं।**

### स्थापना निर्देश

1.  **क्लोन रेपो**

```bash
git clone https://github.com/DrewThomasson/ebook2audiobook.git
```

### लॉन्चिंग ग्रेडियो वेब इंटरफ़ेस

1.  **Ebook2audiobook चलाएं**:
    -   **लिनक्स/मैकओएस**
        ```bash
        ./ebook2audiobook.sh  # Run Launch script
        ```
    -   **खिंचाव**
        ```bash
        .\ebook2audiobook.cmd  # Run launch script or double click on it (Bypass windows alerts)
        ```
2.  **वेब ऐप खोलें**: वेब ऐप तक पहुंचने और ई -बुक्स को कन्वर्ट करने के लिए टर्मिनल में प्रदान किए गए URL पर क्लिक करें।
3.  **सार्वजनिक कड़ी के लिए**:`python app.py --share`(सभी ओएस)`./ebook2audiobook.sh --share`(लिनक्स/मैकओएस)`ebook2audiobook.cmd --share`(विंडोज)

> [!महत्वपूर्ण]**यदि स्क्रिप्ट को रोका जाता है और फिर से चलाया जाता है, तो आपको अपने ग्रैडियो जीयूआई इंटरफ़ेस को ताज़ा करने की आवश्यकता है<br>वेब पेज को नए कनेक्शन सॉकेट को फिर से जोड़ने दें।**

### मूल उपयोग

-   **लिनक्स/मैकओएस**:
    ```bash
    ./ebook2audiobook.sh --headless --ebook <path_to_ebook_file> \
        --voice [path_to_voice_file] --language [language_code]
    ```
-   **खिंचाव**
    ```bash
    .\ebook2audiobook.cmd --headless --ebook <path_to_ebook_file>
        --voice [path_to_voice_file] --language [language_code]
    ```
-   **[--ईबुक]**: अपनी ईबुक फ़ाइल के लिए पथ।
-   **[--आवाज़]**: वॉयस क्लोनिंग फ़ाइल पथ (वैकल्पिक)।
-   **[--भाषा]**: ISO-639-3 में भाषा कोड (यानी: इटैलियन के लिए ITA, अंग्रेजी के लिए ENG, जर्मन के लिए DEU ...)।<br>डिफ़ॉल्ट भाषा ENG और -भाषा में डिफ़ॉल्ट भाषा सेट के लिए वैकल्पिक है ।/lib/lang.py।<br>ISO-639-1 2 अक्षर कोड भी समर्थित हैं।

### कस्टम मॉडल ज़िप अपलोड का उदाहरण

।

-   **लिनक्स/मैकओएस**
    ```bash
    ./ebook2audiobook.sh --headless --ebook <ebook_file_path> \
        --voice <target_voice_file_path> --language <language> --custom_model <custom_model_path>
    ```
-   **खिंचाव**
    ```bash
    .\ebook2audiobook.cmd --headless --ebook <ebook_file_path> \
        --voice <target_voice_file_path> --language <language> --custom_model <custom_model_path>
    ```
-   **&lt;custom_model_path>**: पथ`model_name.zip`फ़ाइल,
        जिसमें सभी अनिवार्य फाइलें शामिल होंगी (टीटीएस इंजन के अनुसार)<br>(देखें ./lib/models.py)।

### उपयोग करने के लिए सभी मापदंडों की सूची के साथ विस्तृत गाइड के लिए

-   **लिनक्स/मैकओएस**
    ```bash
    ./ebook2audiobook.sh --help
    ```
-   **खिंचाव**
    ```bash
    .\ebook2audiobook.cmd --help
    ```
-   **या सभी ओएस के लिए**
    ```python
     app.py --help
    ```

<a id="help-command-output"></a>

```bash
usage: app.py [-h] [--script_mode SCRIPT_MODE] [--session SESSION] [--share]
              [--headless] [--ebook EBOOK] [--ebooks_dir EBOOKS_DIR]
              [--language LANGUAGE] [--voice VOICE] [--device {cpu,gpu,mps}]
              [--tts_engine {xtts,bark,vits,fairseq,yourtts}]
              [--custom_model CUSTOM_MODEL] [--fine_tuned FINE_TUNED]
              [--output_format OUTPUT_FORMAT] [--temperature TEMPERATURE]
              [--length_penalty LENGTH_PENALTY] [--num_beams NUM_BEAMS]
              [--repetition_penalty REPETITION_PENALTY] [--top_k TOP_K] [--top_p TOP_P]
              [--speed SPEED] [--enable_text_splitting] [--output_dir OUTPUT_DIR]
              [--version]

Convert eBooks to Audiobooks using a Text-to-Speech model. You can either launch the Gradio interface or run the script in headless mode for direct conversion.

options:
  -h, --help            show this help message and exit
  --session SESSION     Session to resume the conversion in case of interruption, crash, 
                            or reuse of custom models and custom cloning voices.

**** The following option are for gradio/gui mode only:
  Optional

  --share               Enable a public shareable Gradio link.

**** The following options are for --headless mode only:
  --headless            Run the script in headless mode
  --ebook EBOOK         Path to the ebook file for conversion. Cannot be used when --ebooks_dir is present.
  --ebooks_dir EBOOKS_DIR
                        Relative or absolute path of the directory containing the files to convert. 
                            Cannot be used when --ebook is present.
  --language LANGUAGE   Language of the e-book. Default language is set 
                            in ./lib/lang.py sed as default if not present. All compatible language codes are in ./lib/lang.py

optional parameters:
  --voice VOICE         (Optional) Path to the voice cloning file for TTS engine. 
                            Uses the default voice if not present.
  --device {cpu,gpu,mps}
                        (Optional) Pprocessor unit type for the conversion. 
                            Default is set in ./lib/conf.py if not present. Fall back to CPU if GPU not available.
  --tts_engine {xtts,bark,vits,fairseq,yourtts}
                        (Optional) Preferred TTS engine (available are: ['xtts', 'bark', 'vits', 'fairseq', 'yourtts'].
                            Default depends on the selected language. The tts engine should be compatible with the chosen language
  --custom_model CUSTOM_MODEL
                        (Optional) Path to the custom model zip file cntaining mandatory model files. 
                            Please refer to ./lib/models.py
  --fine_tuned FINE_TUNED
                        (Optional) Fine tuned model path. Default is builtin model.
  --output_format OUTPUT_FORMAT
                        (Optional) Output audio format. Default is set in ./lib/conf.py
  --temperature TEMPERATURE
                        (xtts only, optional) Temperature for the model. 
                            Default to config.json model. Higher temperatures lead to more creative outputs.
  --length_penalty LENGTH_PENALTY
                        (xtts only, optional) A length penalty applied to the autoregressive decoder. 
                            Default to config.json model. Not applied to custom models.
  --num_beams NUM_BEAMS
                        (xtts only, optional) Controls how many alternative sequences the model explores. Must be equal or greater than length penalty. 
                            Default to config.json model.
  --repetition_penalty REPETITION_PENALTY
                        (xtts only, optional) A penalty that prevents the autoregressive decoder from repeating itself. 
                            Default to config.json model.
  --top_k TOP_K         (xtts only, optional) Top-k sampling. 
                            Lower values mean more likely outputs and increased audio generation speed. 
                            Default to config.json model.
  --top_p TOP_P         (xtts only, optional) Top-p sampling. 
                            Lower values mean more likely outputs and increased audio generation speed. Default to 0.85
  --speed SPEED         (xtts only, optional) Speed factor for the speech generation. 
                            Default to config.json model.
  --enable_text_splitting
                        (xtts only, optional) Enable TTS text splitting. This option is known to not be very efficient. 
                            Default to config.json model.
  --output_dir OUTPUT_DIR
                        (Optional) Path to the output directory. Default is set in ./lib/conf.py
  --version             Show the version of the script and exit

Example usage:    
Windows:
    Gradio/GUI:
    ebook2audiobook.cmd
    Headless mode:
    ebook2audiobook.cmd --headless --ebook '/path/to/file'
Linux/Mac:
    Gradio/GUI:
    ./ebook2audiobook.sh
    Headless mode:
    ./ebook2audiobook.sh --headless --ebook '/path/to/file'
```

नोट: Gradio/GUI मोड में, रनिंग रूपांतरण को रद्द करने के लिए, बस पर क्लिक करें[एक्स]Ebook अपलोड घटक से।

### डॉकर का उपयोग करना

आप ईबुक को ऑडियोबुक कनवर्टर को चलाने के लिए डॉकर का उपयोग भी कर सकते हैं। 
यह विधि विभिन्न वातावरणों में स्थिरता सुनिश्चित करती है और सेटअप को सरल करती है।

#### डॉकर कंटेनर चलाना

डॉकर कंटेनर को चलाने और ग्रेडियो इंटरफ़ेस शुरू करने के लिए, निम्न कमांड का उपयोग करें:

\-पू के साथ ही

```powershell
docker run --rm -p 7860:7860 athomasson2/ebook2audiobook
```

Gpu स्पीडअप के साथ -रन (केवल NVIDIA संगत)

```powershell
docker run --rm --gpus all -p 7860:7860 athomasson2/ebook2audiobook
```

#### डॉकर कंटेनर का निर्माण

-   आप कमांड के साथ डॉकर छवि बना सकते हैं:

```powershell
docker build --platform linux/amd64 -t athomasson2/ebook2audiobook .
```

यह कमांड पोर्ट 7860 पर ग्रैडियो इंटरफ़ेस शुरू करेगा। (लोकलहोस्ट: 7860)

-   अधिक विकल्पों के लिए पैरामीटर जोड़ें`--help`

## डॉकर कंटेनर फ़ाइल स्थान

सभी ebook2audiobooks के पास आधार dir होगा`/home/user/app/`उदाहरण के लिए:`tmp`=`/home/user/app/tmp``audiobooks`=`/home/user/app/audiobooks`

## डॉकर हेडलेस गाइड

पहले के साथ नवीनतम के एक डॉकर पुल के लिए

```bash
docker pull athomasson2/ebook2audiobook
```

-   इससे पहले कि आप इसे चलाएं
    जिसे लिंक किया जाएगा, यह वह जगह है जहाँ आप अपनी इनपुट फ़ाइलों को देखने के लिए डॉकर छवि के लिए रख सकते हैं

```bash
mkdir input-folder && mkdir Audiobooks
```

-   नीचे दिए गए कमांड में स्वैप आउट**Your_input_file.txt**आपकी इनपुट फ़ाइल के नाम के साथ

```bash
docker run --rm \
    -v $(pwd)/input-folder:/home/user/app/input_folder \
    -v $(pwd)/audiobooks:/home/user/app/audiobooks \
    athomasson2/ebook2audiobook \
    --headless --ebook /input_folder/YOUR_EBOOK_FILE
```

-   और यह होना चाहिए!
-   आउटपुट ऑडियोबुक को ऑडियोबुक फ़ोल्डर में मिलेगा जो भी स्थित होगा
    अपने स्थानीय dir में आपने इस डॉकर कमांड को चलाया

## अन्य मापदंडों के लिए सहायता कमांड प्राप्त करने के लिए यह कार्यक्रम आप इसे चला सकते हैं

```bash
docker run --rm athomasson2/ebook2audiobook --help

```

और यह आउटपुट होगा[कमांड आउटपुट में मदद करें](#help-command-output)

### डॉकर रचना

यह परियोजना स्थानीय रूप से चलाने के लिए डॉकर की रचना का उपयोग करती है। आप GPU समर्थन को सक्षम या अक्षम कर सकते हैं 
या तो सेट करके`*gpu-enabled`या`*gpu-disabled`में`docker-compose.yml`

#### दौड़ने के लिए कदम

1.  **Clone the Repository**(यदि आप पहले से ही नहीं हैं):
    ```bash
    git clone https://github.com/DrewThomasson/ebook2audiobook.git
    cd ebook2audiobook
    ```
2.  **GPU समर्थन सेट करें (डिफ़ॉल्ट रूप से अक्षम)**GPU समर्थन को सक्षम करने के लिए, संशोधित करें`docker-compose.yml`और बदलें`*gpu-disabled`को`*gpu-enabled`
3.  **सेवा शुरू करें:**
    ```bash
    docker-compose up -d
    ```
4.  **सेवा का उपयोग करें:**सेवा http&#x3A; // localhost: 7860 पर उपलब्ध होगी।

### डॉकर गुई इंटरफ़ेस

![demo_web_gui](assets/demo_web_gui.gif)

<details>
  <summary>Click to see images of Web GUI</summary>
  <img width="1728" alt="GUI Screen 1" src="assets/gui_1.png">
  <img width="1728" alt="GUI Screen 2" src="assets/gui_2.png">
  <img width="1728" alt="GUI Screen 3" src="assets/gui_3.png">
</details>

## एक GPU किराए पर लेना

इसे चलाने के लिए हार्डवेयर नहीं है या आप एक GPU किराए पर लेना चाहते हैं?

#### आप ह्यूगिनफेस स्पेस को डुप्लिकेट कर सकते हैं और लगभग $ 0.40 प्रति घंटे के लिए एक GPU किराए पर ले सकते हैं

[हगिंग स्पेस डेमो](#huggingface-space-demo)

#### या आप मुफ्त में Google Colab का उपयोग करने का प्रयास कर सकते हैं!

(इस बात से अवगत रहें[नि: शुल्क Google Colab](#free-google-colab)

## सामान्य डॉकर मुद्दे

-   Docker ठीक ट्यून किए गए मॉडल डाउनलोड करने के लिए अटक जाता है।
    (यह हर कंप्यूटर के लिए नहीं होता है, लेकिन कुछ इस मुद्दे पर चलते हैं)
    प्रगति बार को अक्षम करना समस्या को ठीक करने के लिए प्रकट होता है,
    चर्चा के अनुसार[यहाँ #191 में](https://github.com/DrewThomasson/ebook2audiobook/issues/191)में इस फिक्स को जोड़ने का उदाहरण`docker run`आज्ञा

```Dockerfile
docker run --rm --gpus all -e HF_HUB_DISABLE_PROGRESS_BARS=1 -e HF_HUB_ENABLE_HF_TRANSFER=0 \
    -p 7860:7860 athomasson2/ebook2audiobook
```

## ठीक ट्यून टीटीएस मॉडल

आप इस रेपो के साथ आसानी से अपने स्वयं के XTTs मॉडल को ठीक कर सकते हैं[Xtts-finetune-webui](https://github.com/daswer123/xtts-finetune-webui)

यदि आप एक GPU को आसानी से किराए पर लेना चाहते हैं तो आप इस हगिंगफेस को भी डुप्लिकेट कर सकते हैं[XTTS-FINETUNE-WEBUI- स्थान](https://huggingface.co/spaces/drewThomasson/xtts-finetune-webui-gpu)

एक स्थान जिसे आप प्रशिक्षण डेटा को भी आसानी से डी-नोज़ करने के लिए उपयोग कर सकते हैं[डेनोइज-हगिंगफेस-स्पेस](https://huggingface.co/spaces/drewThomasson/DeepFilterNet2_no_limit)

### ठीक ट्यून टीटीएस संग्रह

पहले से ही ठीक ट्यून किए गए टीटीएस मॉडल के हमारे संग्रह को खोजने के लिए,
मिलने जाना[यह हगिंग फेस लिंक](https://huggingface.co/drewThomasson/fineTunedTTSModels/tree/main)एक XTTS कस्टम मॉडल के लिए आवाज संदर्भ का एक रेफ ऑडियो क्लिप अनिवार्य है:

## क़ौम

**बारिश की आवाज**<https://github.com/user-attachments/assets/d25034d9-c77f-43a9-8f14-0d167172b080>

**डेविड एटनबोरो आवाज**<https://github.com/user-attachments/assets/0d437a41-0b0d-48ed-8c9b-02763d5e48ea>

## समर्थित ईबुक प्रारूप

-   `.epub`,`.pdf`,`.mobi`,`.txt`,`.html`,`.rtf`,`.chm`,`.lit`,`.pdb`,`.fb2`,`.odt`,`.cbr`,`.cbz`,`.prc`,`.lrf`,`.pml`,`.snb`,`.cbc`,`.rb`,`.tcr`
-   **सर्वोत्तम परिणाम**:`.epub`या`.mobi`स्वचालित अध्याय का पता लगाने के लिए

## उत्पादन

-   बनाता है`['m4b', 'm4a', 'mp4', 'webm', 'mov', 'mp3', 'flac', 'wav', 'ogg', 'aac']`मेटाडेटा और अध्यायों के साथ (lib/conf.py) फ़ाइल में सेट करें।
-   **उदाहरण**![Example](https://github.com/DrewThomasson/VoxNovel/blob/dc5197dff97252fa44c391dc0596902d71278a88/readme_files/example_in_app.jpeg)

## सामान्य मुद्दे:

-   CPU धीमा है (सर्वर SMP CPU पर बेहतर है) जबकि NVIDIA GPU में लगभग वास्तविक समय रूपांतरण हो सकता है।[इस बारे में चर्चा](https://github.com/DrewThomasson/ebook2audiobook/discussions/19#discussioncomment-10879846)तेजी से बहुभाषी पीढ़ी के लिए मैं अपने अन्य सुझाव दूंगा[प्रोजेक्ट जो पाइपर-टीटीएस का उपयोग करता है](https://github.com/DrewThomasson/ebook2audiobookpiper-tts)बजाय
    (हालांकि इसमें शून्य-शॉट वॉयस क्लोनिंग नहीं है, और सिरी गुणवत्ता की आवाज है, लेकिन यह सीपीयू पर बहुत तेज है)।
-   "मुझे निर्भरता के मुद्दे हैं" - बस डॉकर का उपयोग करें, इसकी पूरी तरह से निहित है और एक हेडलेस मोड है,
     जोड़ना`--help`अधिक जानकारी के लिए डॉकर रन कमांड के अंत में पैरामीटर।
-   "Im एक काटे गए ऑडियो मुद्दा हो रहा है!" - कृपया इसका एक मुद्दा बनाएं,
     हम हर भाषा नहीं बोलते हैं और उपयोगकर्ताओं से सलाह देने की आवश्यकता है कि वाक्य बंटवारे के तर्क को ठीक करें।

## मुझे क्या मदद चाहिए! 🙌

## [चीजों की पूरी सूची यहां पाई जा सकती है](https://github.com/DrewThomasson/ebook2audiobook/issues/32)

-   उचित वाक्य विभाजन के तरीकों के साथ मदद करने के लिए किसी भी समर्थित भाषाओं में से किसी भी लोगों की मदद
-   संभावित रूप से कई भाषाओं के लिए README गाइड बनाना (क्योंकि एकमात्र भाषा जो मुझे पता है वह अंग्रेजी 😔 है)

## विशेष धन्यवाद

-   **खाना पकाने के टीटी**:[कोक्वि टीटीएस गिथुब](https://github.com/idiap/coqui-ai-TTS)
-   **बुद्धि का विस्तार**:[कैलिबर वेबसाइट](https://calibre-ebook.com)
-   **FFmpeg**:[FFMPEG वेबसाइट](https://ffmpeg.org)
-   [बेहतर अध्याय बचत विधि के लिए @shakenbake15](https://github.com/DrewThomasson/ebook2audiobook/issues/8)

### [विरासत v1.0](legacy/v1.0)

आप कोड देख सकते हैं[यहाँ](legacy/v1.0).

## हमारे सर्वर में शामिल हों!

[![Discord](https://dcbadge.limes.pink/api/server/https://discord.gg/63Tv3F65k6)](https://discord.gg/63Tv3F65k6)
