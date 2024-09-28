![364748453-c1f81d69-6928-4e23-934c-d99dc888f6b1](https://github.com/user-attachments/assets/e1cf0c71-c8f8-4861-a41a-098093a4c8ca)


# TEMU

### **TEMU**(Team + Music)는 기술과 교육을 음악으로 연결하는 혁신적인 음악 생성 서비스를 제공하기 위해 노력하고 있습니다.

---

## **서비스 소개: M.U.T.E**

M.U.T.E (Music, Understanding, Teaching, Education)는 기술, 교육, 음악을 결합하여 어린이들의 학습 경험을 향상시키기 위한 혁신적인 교육 플랫폼입니다. 최첨단 AI 기술인 대규모 언어 모델(LLM)과 음악 생성 AI를 활용해, 어린이들이 단어를 더 쉽고 재미있게 습득할 수 있도록 도와주는 교육용 동요를 생성합니다.

---

## **주제 선정 배경**

M.U.T.E는 음악이 교육에 미치는 긍정적인 효과에 기반하여 개발되었습니다:

- **음악을 통한 학습 도구**: 연구에 따르면 노래를 부르거나 음악 활동에 참여하는 것은 어휘력 향상, 이해력, 표현력에 큰 도움을 주며, 학습 장애를 겪는 어린이들에게 특히 효과적입니다.
  
- **음악 기반 학습의 효과성**: Gordon, Orff, Kodály와 같은 교육학자들은 유아기에 음악 교육이 감정 표현과 인지 발달, 학습 향상에 중요한 역할을 한다고 주장하였습니다. 특히 노래를 활용한 수업은 언어 학습과 같은 과목에서 학업 성취도와 학습 태도를 크게 개선하는 것으로 밝혀졌습니다.

---

## **대상**

M.U.T.E는 다음과 같은 사용자들을 위해 설계되었습니다:

- **어린이**: 어휘 학습과 암기에 도움이 필요한 어린이
- **교사와 학부모**: 노래를 통해 학습을 더욱 재미있게 만들어주고자 하는 교육자
- **자기주도 학습자**: 재미있고 상호작용적인 방식으로 지식을 습득하고자 하는 학생

---

## **주요 기능**

1. **키워드 기반 교육용 동요 생성**: 사용자가 학습하고자 하는 단어를 입력하면, AI가 맞춤형 교육 동요를 생성합니다.
2. **음악 공유**: 생성된 동요를 커뮤니티 게시판에 업로드하여 다른 사용자들과 공유할 수 있습니다.

---

## **유저 플로우**

1. 사용자가 학습할 단어 키워드와 동요 스타일을 입력합니다.
2. 시스템이 AI를 통해 동요를 생성하고 다운로드 링크를 제공합니다.
3. 사용자는 생성된 동요를 공유 게시판에 업로드할 수 있습니다.

![User Flow](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F8b6f698e-8a67-4ad1-94b0-53ee956264c9%2Fea8c854d-09b8-4c56-a62d-f9f1f2398930%2Fimage.png?table=block&id=cf47da19-a6f6-456e-b6a1-60d8354a58ad&spaceId=8b6f698e-8a67-4ad1-94b0-53ee956264c9&width=1800&userId=51dd97ed-4b7f-4f0a-bc29-4e7109794d96&cache=v2)

---

## **Sequence Diagram**

![Sequence Diagram*](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F8b6f698e-8a67-4ad1-94b0-53ee956264c9%2F4988c6e8-5e4f-4884-b2ea-c2a8d4941930%2Fimage.png?table=block&id=b12e5f0f-a5b7-4a5b-bde7-f38bb2dc41b7&spaceId=8b6f698e-8a67-4ad1-94b0-53ee956264c9&width=1340&userId=51dd97ed-4b7f-4f0a-bc29-4e7109794d96&cache=v2)

---

## **ERD**

<img width="1142" alt="스크린샷 2024-09-05 오후 8 10 46" src="https://github.com/user-attachments/assets/f514b68a-c27a-4151-be85-0b7cdb58a9ed">


---

## **Cloud Architecture**

![Cloud Architecture](https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F8b6f698e-8a67-4ad1-94b0-53ee956264c9%2F91ff88c8-b547-46f6-befa-586985f3319c%2Fimage.png?table=block&id=1073ac76-91d3-4b56-aea4-36620996f3ae&spaceId=8b6f698e-8a67-4ad1-94b0-53ee956264c9&width=1800&userId=51dd97ed-4b7f-4f0a-bc29-4e7109794d96&cache=v2)

---

## **기술 스택**

- **프론트엔드**: Next.js
- **백엔드**: Nest.js, PostgreSQL
    - [BE API 명세서](http://15.165.232.148:3000/api#/songs)
- **AI 통합**: Flask, LLM(OpenAI API), [Suno API](https://github.com/gcui-art/suno-api/)
    - [AI API 명세서](https://suno.gcui.ai/docs)
- **클라우드 인프라**: AWS (VPC, EC2, S3, RDS, ECR), Docker, Jenkins (CI/CD)

| **구분**      | **기술**        |
| ------------- | --------------- |
| 프론트엔드    | <img src="https://img.shields.io/badge/NextJS-000000?style=flat-square&logo=Next.js&logoColor=white"/>         |
| 백엔드           | <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=NestJS&logoColor=white"/> <img src="https://img.shields.io/badge/TypeORM-FE0803?style=flat-square&logo=typeorm&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white"/>         |
| AI  | <img src="https://img.shields.io/badge/flask-48b0c3?style=flat-square&logo=flask&logoColor=white"/>   <img src="https://img.shields.io/badge/openai-412991?style=flat-square&logo=openai&logoColor=white"/> <img src="https://img.shields.io/badge/suno-ff4b4b?style=flat-square&logo=suno&logoColor=white"/>   |
| 클라우드(인프라)  | <img src="https://img.shields.io/badge/AmazonEC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white"/>  <img src="https://img.shields.io/badge/AmazonS3-569A31?style=flat-square&logo=AmazonS3&logoColor=white"/> <img src="https://img.shields.io/badge/AmazonRDS-527FFF?style=flat-square&logo=amazonrds&logoColor=white"/> <img src="https://img.shields.io/badge/docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>  <img src="https://img.shields.io/badge/jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white"/>      |

---

## **팀 소개: TEMU (Team + Music)**

TEMU는 음악을 통해 기술과 교육을 연결하는 혁신적인 음악 생성 서비스를 제공하기 위해 노력하는 팀입니다.

- **Toby.Kim (김대현)** - 팀장 / AI
- **KC.Kim (김찬영)** - AI
- **Jayden.Jeon (전종건)** - 풀스택(FE)
- **Nunu.Gu (구연우)** - 풀스택(BE)
- **Lyle.Kim (김승주)** - 클라우드
- **Uno.Hann (한윤호)** - 클라우드 (발표)

## 해커톤 발표 자료
[26_TEMU_해커톤_발표자료.pdf](https://github.com/user-attachments/files/16915264/26_TEMU_._.pdf)

