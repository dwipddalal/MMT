# MMT: A Multilingual and Multi-Topic Indian Social Media Dataset

**Dwip Dalal, Vivek Srivastava, and Mayank Singh** · **C3NLP at EACL 2023** · Pages 47–52

[Published paper](https://aclanthology.org/2023.c3nlp-1.6/) · [Searchable PDF](https://aclanthology.org/2023.c3nlp-1.6.pdf) · [arXiv](https://arxiv.org/abs/2304.00634) · [Dataset access](https://huggingface.co/datasets/LingoIITGN/MMT) · [BibTeX](CITATION.bib)

MMT is an **Indian social media dataset for multilingual topic modeling and language identification**, including code-mixed text such as Hindi–English (Hinglish). The paper introduces a Twitter corpus of **1,755,145 tweets**, organized into **13 coarse-grained topics and 63 fine-grained subtopics**, and **MMT-LID**, a subset of **5,346 tweets with human-annotated language labels**.

This is the authors' existing sample-data repository. The paper's full collection sizes are different from the sample sizes available here; the [Lingo Research Group's Hugging Face dataset card](https://huggingface.co/datasets/LingoIITGN/MMT) provides the current release and access instructions.

## Research tasks and language coverage

The paper evaluates **topic modeling** with Latent Dirichlet Allocation (LDA) and contextual topic models, and **language identification** on multilingual and code-mixed Indian Twitter text. It examines how language-identification tools handle code-mixing and how topic models perform across languages and topics.

The original corpus contains 47 language tags assigned by Twitter; these are automatic labels, not a claim of human-verified coverage of 47 languages. The paper discusses English, Hindi, Bengali, Gujarati, Marathi, Telugu, and other languages. MMT-LID includes human corrections and code-mixed language tags, including Hinglish.

## Repository contents and dataset access

| Resource | Contents |
| --- | --- |
| [MMT.json](MMT.json) | 630 sample records, with `tweet`, `language`, `topic_name`, and `sub_topic` fields. |
| [MMT-LID.json](MMT-LID.json) | 100 sample records, including original language tags, correctness judgments, and corrected language labels. |
| [500_word_frequency_table.json](500_word_frequency_table.json) | A frequency table for 500 words. |
| [Word Clouds](Word%20Clouds/) | Existing word-cloud visualizations. |
| [Hugging Face dataset](https://huggingface.co/datasets/LingoIITGN/MMT) | The lab's current release, dataset card, access instructions, and terms. |

The JSON samples use a column-oriented format: each field maps row identifiers to values. These sample files are not the complete MMT or MMT-LID datasets. Consult the linked dataset card for the release's access and licensing terms.

## Topics and subtopics

The following table reproduces the paper's distribution of topics, subtopics, tweet counts, and average tweet lengths for the original MMT collection.

| Topic                   | Subtopics                                                                                                                                                                                                                                                                                                                                                 | Tweets | Average length |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ | -------------- |
| Environment             | Pollution, Climate Change, Eco Friendly, Floods                                                                                                                                                                                                                                                                                                           | 142208 | 216.58         |
| Food                    | Online food delivery, Food security, Indian desserts                                                                                                                                                                                                                                                                                                      | 195086 | 140.75         |
| Economics and Retail    | Initial Public Offering (IPO), SEBI and New margin rules, Unicorns, Unemployment in India                                                                                                                                                                                                                                                                 | 158016 | 179.16         |
| Natural Disaster        | Cyclone, Earthquake, Pandemic, Flood                                                                                                                                                                                                                                                                                                                      | 75591  | 161.18         |
| Art and Literature      | Forms of Indian Art, Art festivals, Literature festivals, Book Fairs                                                                                                                                                                                                                                                                                      | 111909 | 150.43         |
| Sports                  | Olympics, Indian Premier League (IPL), Indian Super League (ISL), Pro Kabaddi League (PKL)                                                                                                                                                                                                                                                                | 122740 | 117.06         |
| Politics                | Pegasus Snooping, Farmer Agitation, West Bengal Elections, 2021                                                                                                                                                                                                                                                                                           | 119963 | 155.0          |
| R&D and Technology      | Mobile Technology, Health-Tech and Medical Innovations, ISRO                                                                                                                                                                                                                                                                                              | 111615 | 166.43         |
| Wildlife and Vegetation | Kaziranga National Park, Bandhavgarh National Park, Nilgiri National Park, Corbett National Park, Ranthambore National Park, Gir National Park, Nanda Devi National Park, Save Tiger Project, Save Elephants, Save the Great Indian Bustard, Wildlife Tourism and Heritage, Forest Cover, River Rejuvenation, Restoration, Wildlife Crime, Climate Change | 280091 | 155.03         |
| Manufacturing           | Make in India, Steel Manufacturing, Automobile Manufacturing, Electronics and electrical manufacturing                                                                                                                                                                                                                                                    | 100969  | 125.14         |
| Films and OTT           | OTT platforms such as Netflix, Amazon Prime Video, etc; OTT Voicecalling; OTT Censorship; Nepotism in Film Industry; National Film Awards                                                                                                                                                                                                                 | 89760  | 142.12         |
| Journalism & Media      | Policy and Trends, Print Media & TV, Criminal Journalism, Social Movements and News                                                                                                                                                                                                                                                                       | 139563 | 170.88         |
| Education               | Exams, IIT, Online Education, Education System                                                                                                                                                                                                                                                                                                            | 107634 | 186.39         |

## Citation

If you use MMT, MMT-LID, or the accompanying samples, please cite the published paper:

Dwip Dalal, Vivek Srivastava, and Mayank Singh. 2023. [MMT: A Multilingual and Multi-Topic Indian Social Media Dataset](https://aclanthology.org/2023.c3nlp-1.6/). In *Proceedings of the First Workshop on Cross-Cultural Considerations in NLP (C3NLP)*, pages 47–52, Dubrovnik, Croatia. Association for Computational Linguistics. DOI: [10.18653/v1/2023.c3nlp-1.6](https://doi.org/10.18653/v1/2023.c3nlp-1.6).

The [arXiv preprint (2304.00634)](https://arxiv.org/abs/2304.00634) and the C3NLP 2023 publication describe the same work. Use the published 2023 citation below. [CITATION.bib](CITATION.bib) preserves ACL Anthology's BibTeX entry and citation key, `dalal-etal-2023-mmt`.

<!-- The BibTeX below is copied from ACL Anthology; keep it in sync with CITATION.bib. -->

```bibtex
@inproceedings{dalal-etal-2023-mmt,
    title = "{MMT}: A Multilingual and Multi-Topic {I}ndian Social Media Dataset",
    author = "Dalal, Dwip  and
      Srivastava, Vivek  and
      Singh, Mayank",
    editor = "Dev, Sunipa  and
      Prabhakaran, Vinodkumar  and
      Adelani, David Ifeoluwa  and
      Hovy, Dirk  and
      Benotti, Luciana",
    booktitle = "Proceedings of the First Workshop on Cross-Cultural Considerations in NLP (C3NLP)",
    month = may,
    year = "2023",
    address = "Dubrovnik, Croatia",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.c3nlp-1.6/",
    doi = "10.18653/v1/2023.c3nlp-1.6",
    pages = "47--52"
}
```
