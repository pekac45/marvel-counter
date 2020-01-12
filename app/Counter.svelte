<script>
  export let counter = 42;
</script>

<style>
  .h1 {
    font-size: 100;
    color: #333;
    margin-top: 100;
  }

  .btn {
    border-radius: 30%;
    color: #fff;
  }

  .success {
    background-color: #22bb33;
  }

  .danger {
    background-color: #bb2124;
  }

  .coverImage {
    background-image: url("~/bg.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
  }
</style>

<flexboxLayout
  class="p-20 coverImage"
  flexDirection="column"
  justifyContent="center">
  <label text={counter} class="h1 text-center" backgroundColor="" />
  <flexboxLayout class="p-20" alignContent="flex-end" justifyContent="center">

    <button
      text="-1"
      on:tap={() => (counter = counter - 1)}
      class="danger btn"
      width="100" />
    <button
      text="-5"
      on:tap={() => (counter = counter - 5)}
      class="danger btn"
      width="100" />
    <button
      text="-10"
      on:tap={() => (counter = counter - 10)}
      class="danger btn"
      width="100" />

    <button
      text="+10"
      on:tap={() => (counter = counter + 10)}
      class="success btn"
      width="100" />
    <button
      text="+5"
      on:tap={() => (counter = counter + 5)}
      class="success btn"
      width="100" />
    <button
      text="+1"
      on:tap={() => (counter = counter + 1)}
      class="success btn"
      width="100" />
  </flexboxLayout>
</flexboxLayout>
