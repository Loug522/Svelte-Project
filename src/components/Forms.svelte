<script>
  const uid = $props.id();
</script>

<div class="wrapper">
  <form>
    <label for="{uid}-firstName">First Name:</label>
    <input id="{uid}-firstName" type="text" />

    <label for="{uid}-lastName">Last Name:</label>
    <input id="{uid}-lastName" type="text" />

    <label for="{uid}-age">Age:</label>
    <input id="{uid}-age" type="number" />

    <fieldset class="gender-container">
      <legend>Gender</legend>
      <input id="{uid}-genderMale" name="gender" type="radio" checked />
      <label for="{uid}-genderMale">Male</label>

      <input id="{uid}-genderFemale" name="gender" type="radio" />
      <label for="{uid}-genderFemale">Female</label>

      <input id="{uid}-genderOther" name="gender" type="radio" />
      <label for="{uid}-genderOther">Other</label>
    </fieldset>

    <button>submit</button>
  </form>
</div>

<style>
  .wrapper {
    padding-block: 1rem;
    padding-inline: 2rem;
  }

  .gender-container,
  .wrapper {
    border: 1px solid hsla(1, 0%, 50%, 0.5);
    border-radius: 1rem;
    box-shadow: 0 0 3px hsla(1, 0%, 50%, 0.3);
  }

  form {
    display: grid;
    text-align: start;

    label {
      margin-block-end: 0.5rem;
    }

    input {
      margin-block-end: 1rem;
    }
  }

  button {
    font-weight: bold;
    text-transform: uppercase;
    margin-block: 1rem;
  }
</style>
