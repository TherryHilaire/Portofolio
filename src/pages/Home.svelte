<script>
    import avatar from "../assets/me.png"
    import setup from "../assets/setup.jpg"
    import Typewriter from 'svelte-typewriter'
</script>

<main>
  <div class="container">
    <div class="picture">
        <img src={avatar} alt="Therry Léonhard Hilaire" class="pic">
        <h1 class="name">Therry Léonhard Hilaire</h1>
        <h3 class="name">Student (Developer in his free time)</h3>
      </div>
      <br />
      <div class="text">
        <Typewriter interval={50}>
          <h2>Good Morning and Welcome.</h2>
          <h2>My name is Therry and I am a student in Haiti. I do programming in my free time. </h2>
          <h3>I love Art, Music, Drawing and Computer Stuff<h3>
        </Typewriter>
      </div>
      <br />
      <div class="about">
        <h3 class="title">More About Me</h3>
        <h3>
        I am a student in a High School in haiti. I have a passion for building anything beautiful and thoughtful. I am in love with art, Music and everthing 
        that surrounds that. When I am not working or programming, I usually go and hang out in my backyard, listen to Music, try to write a little or read a book.
        I have no project that is in a usable state. Because of the current situation of Haiti, I am limited in my freedom (I cannot leave my house safely) and in what Software
        I can use to deploy or for a database, also my computer is kinda weak.
        </h3>
      </div>
      <div class="el_set">
          <h3 class="title">My setup</h3>
          <div class="setup">
          <img src={setup} alt="setup" class="setup-img"/>
          <h3 class="setup-text">
          I am using a MacBookPro late 2013 with Fedora 37. In the picture you can see I am using a hard drive scotched to my pc; It's because my disk is not working so 
          I have no other choice but to use this as my drive. My code editor is Neovim. I code in my bedroom.
        </h3>
      </div>
    </div>
    <div>
        <h3 class="title">Things I like</h3>
        <h3>I love anything that is Artistic (yes that includes Video Games). I love programming in my free time because I found it fun, I also like watching videos on the topic 
        (Like ThePrimeagen). Outside of computers and programming I am pretty curious when it comes to science and stuff like that.</h3>
        <h3>I don't play video games because I don't have time to do so, and when I do have time I don't know what to play (mostly because my computer is weak).</h3>
    </div>
  </div>
</main>

<style>
.title {
    color: grey;
    font-size: 25px; 
    text-decoration: underline;
    padding-left: 10px;
}

.setup-text {
    grid-column-start: 3;
    grid-column-end: 4;
    grid-row-start: 1;
    grid-row-end: 3;
    width: 50%;
}

.setup-img {
    grid-row-start: 1;
    grid-row-end: 3;
}

.setup {
    display: grid;
    column-gap: 6px;
}

.setup-img {
    border-radius: 14px;
    width: 440px;
    height: 300px;
}

h2 {
    font-size: 19px;
}

.pic {
    display: block;
    height: 200px;
    width: 200px;
    border-radius: 120px;
    margin-left: 520px;
}

.text {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 50%;
}

.name {
    border: none!important; 
    text-align: center;
    display: block;
}
</style>
