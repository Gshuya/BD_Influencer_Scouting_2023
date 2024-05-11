# Influencer_Scouting
Reference: "Multimodal Post Attentive Profiling for Influencer Marketing," Seungbae Kim, Jyun-Yu Jiang, Masaki Nakada, Jinyoung Han and Wei Wang. In Proceedings of The Web Conference (WWW '20), ACM, 2020.

<img width="624" alt="Screenshot 2024-05-11 at 20 27 45" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/d1c7430a-a014-45c7-852e-9b54fc83022f">

## Post Embedding: feature extraction

<img width="520" alt="Screenshot 2024-05-11 at 20 44 59" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/160d32d1-8a48-4fff-908b-248e571ef36f">
<img width="520" alt="Screenshot 2024-05-11 at 20 29 37" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/68770741-cf6b-454f-baa4-17cef075880d">
<img width="520" alt="Screenshot 2024-05-11 at 20 29 54" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/d387f4eb-89b9-4b0d-b69a-ea803ee79be0">

## Influencer embedding
1. Aggregate all post features by averaging values
<img width="520" alt="Screenshot 2024-05-11 at 20 34 02" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/5607a93c-4c94-4168-838c-434149e07194">

<img width="520" alt="Screenshot 2024-05-11 at 20 34 29" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/452ce25d-1c0a-488b-8e35-4d70eae3ce21">

2. Use attention mechanism to weigh higher scores on more important posts
<img width="520" alt="Screenshot 2024-05-11 at 20 38 55" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/0b46cf66-c123-45a0-a056-b6f6825143c7">

## Classification
1. PySpark models (LogisticRegression, Random Forest, GaussianNaïveBayes) with simple averaged influencer embeddings as input.

2. After applying an attention mechanism, influencer embeddings are passed through one or more fully connected layers to produce the final classification output.
<img width="520" alt="Screenshot 2024-05-11 at 20 40 21" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/1419289f-5187-4f28-91af-d33e09c671e2">

## App Demo
<img width="580" alt="Screenshot 2024-05-11 at 20 41 01" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/989cc9cf-721a-4ef2-b05f-704682e7f2ba">

<img width="580" alt="Screenshot 2024-05-11 at 20 45 44" src="https://github.com/Gshuya/BD_Influencer_Scouting_2023/assets/61619494/aa6c727f-e7ec-4cf1-8a91-cd346c6657a3">
