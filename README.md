### Hi there i'm Muhodari Sage 👋

- E-commerce: https://kha23accessories.netlify.app/                                                                                                                              
- save picture app: https://savepicture.netlify.app/
- vue-simple routing: https://msage-vue-routing.netlify.app/
- vue RFID-transaction app: https://gitash-rfid-nodemcu.netlify.app/
- django rest framework: http://ec2-13-59-87-224.us-east-2.compute.amazonaws.com/api/


<!--
**Muhodari/Muhodari** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->




 const fetcher = (variables, token) => { 
   return request( 
     { 
       query: ` 
       query userInfo($login: String!) { 
         user(login: $login) { 
           repositories(isFork: false, first: 100) { 
             nodes { 
               languages(first: 1) { 
                 edges { 
                   size 
                   node { 
                     color 
                     name 
                   } 
                 } 
               } 
             } 
           } 
         } 
       } 
