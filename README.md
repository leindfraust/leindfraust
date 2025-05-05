<span id="age"></span> yrs old Full Stack Developer from Philippines.

`Next.js | Nuxt.js | Node.js | Express.js | Nest.js`

rozer223@gmail.com

<script>
function calculateAge(birthday) {
  const today = new Date();
  const birthDate = new Date(birthday);
  let age = today.getFullYear() - birthDate.getFullYear();
  const m = today.getMonth() - birthDate.getMonth();
  if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
    age--;
  }
  return age;
}

const birthday = "May 24, 2000";
const yourAge = calculateAge(birthday);

document.getElementById("age").textContent = "Your age is: " + yourAge;
</script>
