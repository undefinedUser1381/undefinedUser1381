# 💻 Frontend Developer | React | Next.js | PWA

![Profile views](https://komarev.com/ghpvc/?username=YOUR_USERNAME&color=blueviolet)
![GitHub followers](https://img.shields.io/github/followers/YOUR_USERNAME?label=Follow&style=social)

## 🚀 Tech Stack

<div align="center">

### 🧩 Main Technologies

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

### 🔧 Tools & Libraries

![React Query](https://img.shields.io/badge/-React%20Query-FF4154?style=for-the-badge&logo=react%20query&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

</div>

---

## 📌 About Me

- 🔭 I’m currently working on **modern frontend projects**
- 🌱 Learning **Next.js 15 + PWA**
- 💬 Ask me about **React, Tailwind, React Query**
- 📫 How to reach me: `your.email@example.com`
- ⚡ Fun fact: I love building fast & beautiful web apps

---

## 🧪 Sample React Query + API

```js
import { useQuery } from '@tanstack/react-query';

const fetchUsers = async () => {
  const res = await fetch('https://jsonplaceholder.typicode.com/users');
  return res.json();
};

export default function Users() {
  const { data, isLoading } = useQuery({ queryKey: ['users'], queryFn: fetchUsers });
  if (isLoading) return <p>Loading...</p>;
  return <ul>{data.map(user => <li key={user.id}>{user.name}</li>)}</ul>;
}
