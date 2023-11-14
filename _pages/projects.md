---
title: Projects
layout: default
permalink: /projects/
published: true
---

## American Sign Language-English Machine Translation

<table>
  <tr>
    <td>
      <img src="{{ '/assets/images/asl-En_diagram.png' | relative_url }}" width="408" height="296"/>      
    </td>
    <td>
      <video width="340" height="288" controls autoplay>
        <source src="{{ '/assets/images/jk_demo_combined_680x576.mp4' | relative_url }}" type="video/mp4" />
      </video>
    </td>
  </tr>
</table>

I worked on a government-funded research and development project that developed a bi-directional communication system between signers and speakers.
I led a team of linguists and engineers and successfully completed the 5-year long project, exploring end-to-end Tranformer and segment-classify-decoding approaches.
The team developed a deep neural network-based sign recognition model that recognizes American Sign language, both sign glosses and fingerspells, and an ASL-English MT model that translates the recognized ASL glosses and fingerspells into English. 
The demo also translated Spoken English into sign glosses and fingerspells that were animated by an avatar.

Here are the links to the research paper and related open source codes from the early stage of the project:
 - [Improving American Sign Language Recognition with Synthetic Data, MT Summit 2019](https://aclanthology.org/W19-6615/)
 - [https://github.com/dragonfly-asl/ASLRFeatureExtractor](https://github.com/dragonfly-asl/ASLRFeatureExtractor)
 - [https://github.com/dragonfly-asl/SyntheticDataGenerator](https://github.com/dragonfly-asl/SyntheticDataGenerator)

The final demo system is not in the public domain (yet?) and is being further refined and maintained by the project sponsor.


## Neural Machine Translation
 - denoising objectives with mono/multilingual text + MT objectives for training NMT (Raffel et al., 2019; Ma et al., 2021; Chi et al., 2021) with Multi-Task, Multi-langpair Learning
 - Document-level LLM Prompt-based MT
 - Tied Transformers (Xia et al., 2019)
 - Retrieval Augmented NMT (Hoang et al., 2023)
 - [Position Encoders for LLM: ALiBi (Press et al., 2022), RoPE (Su et al., 2021), XPOS (Sun et al., 2021)](https://github.com/OpenNMT/OpenNMT-tf/compare/master...jungikim:OpenNMT-tf:rope_alibi)
 - Segment merger, spliter for Dialogue MT
 - [Multimodal (Video, Audio, Text) Transformers](https://github.com/OpenNMT/OpenNMT-tf/compare/master...jungikim:OpenNMT-tf:multimodal)
 - [CTC Decoding with alignment](https://github.com/baidu-research/warp-ctc/compare/master...jungikim:warp-ctc:master)
 - SVD Softmax (Shim et al., 2017) [luatorch](https://github.com/torch/nn/compare/master...jungikim:nn:svdlinear), [Cuda](https://github.com/torch/cunn/compare/master...jungikim:cunn:svdlinear)



## Cross-Language Information Retrieval
 - Learning Semantics with Deep Belief Networks (COLING 2012)
 - Translating Queries with Pseudo-Contextual Information (Unpublished, [PDF](https://drive.google.com/file/d/1tMhYKwKk-Cuw1SBWZgCfcPTfCVRM47p9/view))
 - Cross-lingual Link Discovery
 - Patent CLIR


## Multilingual Natural Language Processing
 - Evaluating Multilanguage-Comparability of Subjectivity Analysis Systems (ACL 2010)
 - Discovering the Discriminative Views: Measuring Term Weights for Sentiment Analysis (ACL-ICJNLP 2009)
 - Conveying Subjectivity of a Lexicon of One Language into Another Using a Bilingual Dictionary and a Link Analysis Algorithm (ICCPOL 2009)


## ...
