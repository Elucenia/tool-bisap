<!-- ELUCENIA technical documentation · bisap · hi · no clinical/professional/rights approval -->

# BISAP स्कोर

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/bisap)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### यूरिया \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### मानसिक स्थिति में बदलाव (Glasgow \< 15)

`mental`

### SIRS (2 या अधिक मानदंड)

`sirs`

### आयु \> 60 वर्ष

`idade`

### इमेजिंग में प्लूरल इफ़्यूज़न

`derrame`

## विधि का संस्करण

BISAP/Wu 2008: 5 कारक, पहले 24 h; BUN \>25 mg/dL; आयु \>60

## दस्तावेज़ित सूत्र

पहले 24 घंटे में हर कारक 1 अंक: BUN \>25 mg/dL (यूरिया \>53 mg/dL), I मानसिक स्थिति बिगड़ी, SIRS, A आयु \>60 वर्ष, P प्लूरल इफ्यूज़न।

SIRS: ≥2 इनमें से तापमान \<36 या \>38 °C, हृदयगति \>90 bpm, श्वसन \>20/मिनट या PaCO₂ \<32 mmHg, श्वेत कोशिकाएँ \<4000 या \>12000/mm³ या \>10% बैंड कोशिकाएँ।

## सीमाएँ और जनसमूह

2008 का BISAP तीव्र अग्नाशयशोथ के पहले 24 घंटे के डेटा से अस्पताल में मृत्यु के जोखिम का स्तरीकरण करता है। BUN \>25 mg/dL और उम्र \>60 वर्ष स्कोर की मदें हैं, शामिल करने की न्यूनतम शर्तें नहीं। नेक्रोसिस, अंग विफलता और उपसमूहों में उपयोग का मूल्यांकन संबंधित स्रोतों पर निर्भर है; देखी गई दरें व्यक्तिगत पूर्वानुमान की निश्चितता नहीं हैं।

## संदर्भ

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026
