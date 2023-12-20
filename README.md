<!-- <img alt="Can Stock Photo www.canstockphoto.com / coraMax.  Used with permission." src="favicon.svg" width="40%"/> -->

# URGENT Challenge: Universality, Robustness, and Generalizability for speech EnhancemeNT
<!-- ## Special session at [Interspeech 2024](https://www.interspeech2024.org)  -->

### Background

Recent decades have witnessed rapid development of deep learning-based speech enhancement (SE) techniques, with impressive performance in matched conditions. However, most conventional speech enhancement approaches focus only on a limited range of conditions, such as single-channel, multi-channel, anechoic, and so on.

Usually, they tend to only train SE models on one or two common datasets, such as the VoiceBank+DEMAND and DNS datasets. The evaluation is often done only on simulated conditions that are similar to the training setting. This greatly impedes understanding of the generalizability and robustness of SE methods comprehensively. In addition, the model design may be biased towards a specific limited condition if only a small amount of data is used. The resultant SE model may also have a limited capacity to handle more complicated scenarios.

Apart from conventional discriminative methods, generative methods have also attracted much attention in recent years. They are good at handling different distortions with a single model [1] and tend to generalize better than discriminative methods [2]. However, their capability and universality have not yet been fully understood through a comprehensive benchmark.

Meanwhile, recent efforts [3] have shown the possibility of building a single system to handle various input formats, such as different sampling frequencies and numbers of microphones. However, there lacks a well-established benchmark covering a wide range of conditions, and no systematic comparison has been made between state-of-the-art (SOTA) discriminative and generative methods regarding their generalizability.

Existing speech enhancement challenges have fostered the development of speech enhancement models for specific conditions, such as denoising [4-8], speech restoration [9], packet loss concealment [10], acoustic echo cancellation [11-13], hearing aid [14-15], 3D speech enhancement [16-17], far-field multi-channel speech enhancement for video conferencing [18], and unsupervised domain adaptation for denoising [19]. These challenges have greatly enriched the corpora in speech enhancement studies. However, there still lacks a challenge that can benchmark the generalizability of speech enhancement systems in a wide range of conditions.

Similar issues can also be observed in other speech tasks such as automatic speech recognition (ASR), speech translation (ST), speaker verification (SV), and spoken language understanding (SLU). Among them, speech enhancement is particularly vulnerable to mismatches since it is heavily reliant on paired clean/noisy speech data to achieve strong performance. Unsupervised speech enhancement that does not require ground-truth clean speech has been proposed to address this issue, but falls short in terms of final performance, while the use of real data for training is not as effective due to the lack of paired clean and noisy data. Therefore, we focus on speech enhancement in this challenge to address the aforementioned problems.


### Goal

Based on the increasing interest in the generalizability of speech enhancement models, we propose the URGENT challenge that aims to:
1. Bring more attention to constructing universal speech enhancement models with strong generalizability.
2. Push forward the progress of speech enhancement research towards more realistic scenarios with a comprehensive evaluation.
3. Provide insightful and systematic comparison between SOTA discriminative and generative methods in a wide range of conditions, including different distortions and input formats (sampling frequencies and number of microphones).
4. Provide a benchmark for this direction so that researchers can easily compare different methods.


### Task

The task is to build a single speech enhancement system to adaptively handle input speech with different distortions (corresponding to different SE subtasks) and different input formats (e.g., sampling frequencies) in different acoustic environments.

We will evaluate models with a variety of metrics to comprehensively understand the capacity of existing generative and discriminative methods.

More details about the data and evaluation plan will be released soon.


### Paper submission

Papers submitted to the session should follow the regular Interspeech paper guidelines, [submission](https://www.interspeech2024.org/paper-submission/) and review process.  <br> 
Accepted papers will appear in the main proceedings and the ISCA archive.  <br>
Be sure to list "URGENT Challenge: Universality, Robustness, and Generalizability for speech EnhancemeNT" as your paper subject area when making a submission. 

**Papers must be submitted by 2 March 2024, but updates are permitted up until 9 March 2024. All dates are Anywhere over Earth (AoE)**

### Organizing team

> The current list is tentative and will be finalized later.

* Wangyou Zhang, Shanghai Jiao Tong University, China
* Robin Scheibler, LINE Corp., Japan
* Samuele Cornell, Carnegie Mellon University, USA
* Chenda Li, Shanghai Jiao Tong University, China
* Kohei Saijo, Waseda University, Japan
* Shinji Watanabe, Carnegie Mellon University, USA


### References

[1] J. Serrà, S. Pascual, J. Pons, R. O. Araz, and D. Scaini, “Universal speech enhancement with score-based diffusion,” arXiv preprint arXiv:2206.03065, 2022.

[2] Y.-J. Lu, Z.-Q. Wang, S. Watanabe, A. Richard, C. Yu, and Y. Tsao, “Conditional diffusion probabilistic model for speech enhancement,” in Proc. IEEE ICASSP, 2022, pp. 7402–7406.

[3] W. Zhang, K. Saijo, Z.-Q. Wang, S. Watanabe, and Y. Qian, “Toward universal speech enhancement for diverse input conditions,” arXiv preprint arXiv:2309.17384, 2023.

[4] C. K. Reddy, V. Gopal, R. Cutler, E. Beyrami, R. Cheng, H. Dubey, S. Matusevych, R. Aichner, A. Aazami, S. Braun, P. Rana, S. Srinivasan, and J. Gehrke, “The INTERSPEECH 2020 deep noise suppression challenge: Datasets, subjective testing framework, and challenge results,” in Proc. ISCA Interspeech, 2020, pp. 2492–2496.

[5] C. K. Reddy, H. Dubey, V. Gopal, R. Cutler, S. Braun, H. Gamper, R. Aichner, and S. Srinivasan, “ICASSP 2021 deep noise suppression challenge,” in Proc. IEEE ICASSP, 2021, pp. 6623–6627.

[6] C. K. Reddy, H. Dubey, K. Koishida, A. Nair, V. Gopal, R. Cutler, S. Braun, H. Gamper, R. Aichner, and S. Srinivasan, “INTERSPEECH 2021 deep noise suppression challenge,” in Proc. ISCA Interspeech, 2021, pp. 2796–2800.

[7] H. Dubey, V. Gopal, R. Cutler, A. Aazami, S. Matusevych, S. Braun, S. E. Eskimez, M. Thakker, T. Yoshioka, H. Gamper, and R. Aichner, “ICASSP 2022 deep noise suppression challenge,” in Proc. IEEE ICASSP, 2022, pp. 9271–9275.

[8] H. Dubey, A. Aazami, V. Gopal, B. Naderi, S. Braun, R. Cutler, A. Ju, M. Zohourian, M. Tang, H. Gamper et al., “ICASSP 2023 deep speech enhancement challenge,” arXiv preprint arXiv:2303.11510, 2023.

[9] R. Cutler, A. Saabas, B. Naderi, N.-C. Ristea, S. Braun, and S. Branets, “ICASSP 2023 speech signal improvement challenge,” arXiv preprint arXiv:2303.06566, 2023.

[10] L. Diener, S. Sootla, S. Branets, A. Saabas, R. Aichner, and R. Cutler, “INTERSPEECH 2022 audio deep packet loss concealment challenge,” in Proc. ISCA Interspeech, 2022, pp. 580–584.

[11]  R. Cutler, A. Saabas, T. Parnamaa, M. Loide, S. Sootla, M. Purin, H. Gamper, S. Braun, K. Sorensen, R. Aichner, and S. Srinivasan, “INTERSPEECH 2021 acoustic echo cancellation challenge,” in Proc. ISCA Interspeech, 2021, pp. 4748–4752.

[12] K. Sridhar, R. Cutler, A. Saabas, T. Parnamaa, M. Loide, H. Gamper, S. Braun, R. Aichner, and S. Srinivasan, “ICASSP 2021 acoustic echo cancellation challenge: Datasets, testing framework, and results,” in Proc. IEEE ICASSP, 2021, pp. 151–155.

[13] R. Cutler, A. Saabas, T. Parnamaa, M. Purin, H. Gamper, S. Braun, K. Sørensen, and R. Aichner, “ICASSP 2022 acoustic echo cancellation challenge,” in Proc. IEEE ICASSP, 2022, pp. 9107–9111.

[14] S. Graetzer, J. Barker, T. J. Cox, M. Akeroyd, J. F. Culling, G. Naylor, E. Porter, and R. V. Muñoz, “Clarity-2021 challenges: Machine learning challenges for advancing hearing aid processing,” in Proc. ISCA Interspeech, 2021, pp. 686–690.

[15] M. A. Akeroyd, W. Bailey, J. Barker, T. J. Cox, J. F. Culling, S. Graetzer, G. Naylor, Z. Podwi'nska, and Z. Tu, “The 2nd clarity enhancement challenge for hearing aid speech intelligibility enhancement: Overview and outcomes,” in Proc. IEEE ICASSP, 2023.

[16] E. Guizzo, R. F. Gramaccioni, S. Jamili, C. Marinoni, E. Massaro, C. Medaglia, G. Nachira, L. Nucciarelli, L. Paglialunga, M. Pennese, S. Pepe, E. Rocchi, A. Uncini, and D. Comminiello, “L3DAS21 challenge: Machine learning for 3D audio signal processing,” in Proc. International Workshop on Machine Learning for Signal Processing (MLSP), 2021, pp. 1–6.

[17] E. Guizzo, C. Marinoni, M. Pennese, X. Ren, X. Zheng, C. Zhang, B. Masiero, A. Uncini, and D. Comminiello, “L3DAS22 challenge: Learning 3D audio sources in a real office environment,” in Proc. IEEE ICASSP, 2022, pp. 9186–9190.

[18] W. Rao, Y. Fu, Y. Hu, X. Xu, Y. Jv, J. Han, Z. Jiang, L. Xie, Y. Wang, S. Watanabe, Z.-H. Tan, H. Bu, T. Yu, and S. Shang, “ConferencingSpeech challenge: Towards far-field multi-channel speech enhancement for video conferencing,” in Proc. IEEE ASRU, 2021, pp. 679–686.

[19] S. Leglaive, L. Borne, E. Tzinis, M. Sadeghi, M. Fraticelli, S. Wisdom, M. Pariente, D. Pressnitzer, and J. R. Hershey, “The CHiME-7 UDASE task: Unsupervised domain adaptation for conversational speech enhancement,” in Proc. 7th International Workshop on Speech Processing in Everyday Environments (CHiME), 2023.

[20] J. Richter, S. Welker, J.-M. Lemercier, B. Lay, and T. Gerkmann, “Speech enhancement and dereverberation with diffusion-based generative models,” IEEE/ACM Trans. ASLP., vol. 31, pp. 2351–2364, 2023.

[21] J. Su, Z. Jin, and A. Finkelstein, “HiFi-GAN: High-fidelity denoising and dereverberation based on speech deep features in adversarial networks,” in Proc. ISCA Interspeech, 2020, pp. 4506–4510.
