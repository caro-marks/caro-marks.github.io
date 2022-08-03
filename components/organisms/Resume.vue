<template>
  <div class="resume my-4">
    <h3>Hi, there! Please to meet me (;</h3>

    <br />
    <h4><strong>Who and where am I?</strong></h4>
    <p>
      I'm Marcos Nolasco, 28-y brazilian, born at Porto Velho - RO, and living
      nowadays at Florianópolis - SC.
    </p>

    <br />
    <h4><strong>What hobbies do I have?</strong></h4>
    <p>
      I've been a compulsive reader since childhood, and I enjoy to watch movies
      a lot.
    </p>

    <br />
    <h4><strong>What do I want most?</strong></h4>
    <p>
      I hope a better world for those who will come, so I wanna help with
      educational status improvement. I also wanna travel all Earth around.
    </p>

    <br />
    <h4><strong>What have I done?</strong></h4>
    <p>
      I graduated at Physics college some months ago. I used to do research
      about complex biophysics systems using Python, and teach classes for Enem
      exams as volunteer.
    </p>
    <br />
    <h4><strong>What have I been doing?</strong></h4>
    <p>
      Since half of 2020 I've been working to become a full-stack developer. I
      did some jobs as backend using Django, and also some personal projects as
      frontend using Vue.
    </p>
    <br />
    <h4><strong>Where am I up to?</strong></h4>
    <p>
      I'm thrilling to be healthier, happier, and to achieve financial freedom.
      Have I said that I wanna travel the world?
    </p>
  </div>
</template>
<style lang="scss" scoped>
p {
  color: color('light');
}
h3 {
  color: color('light', 'darkest')
}
h4 {
  color: rgba(color('light', 'darkest'), 0.75);
  text-shadow: 0px 0px 1px rgba(color('light'), .5),
    0px 0px 2px rgba(color('light','lightest'), 0.25),
    // 0px 0px 1px color('light', 'darkest'),
    // 0px 0px 1px color('light', 'darkest');
}
</style>
