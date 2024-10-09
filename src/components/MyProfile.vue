<template>
  <div class="profile">
    <div class="profile__container">
      <nav class="profile__nav">
        <ul class="list-link">
          <li>
            <a class="link link_active" href="">Edit Profile</a>
          </li>
          <li>
            <a class="link" href="">Preferences</a>
          </li>
          <li>
            <a class="link" href="">Security</a>
          </li>
        </ul>
      </nav>
      <div class="profile__info">
        <div class="foto__container">
          <img class="foto" src="/foto_2.png" alt="foto" />
          <img class="foto__edit" src="/edit.svg" alt="" />
        </div>
        <div class="info">
          <div class="input__box">
            <label for="" class="input__label">Your Name</label>
            <input type="text" class="input" value="Charlene Reed" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">User Name</label>
            <input type="text" class="input" value="Charlene Reed" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Email</label>
            <input type="email" class="input" value="charlenereed@gmail.com " />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Password</label>
            <input type="password" class="input" value="**********" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Date of Birth</label>
            <input type="text" class="input" value="25 January 1990" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Present Address</label>
            <input type="text" class="input" value="San Jose, California, USA" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Permanent Address</label>
            <input type="text" class="input" value="San Jose, California, USA" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">City</label>
            <input type="text" class="input" value="San Jose" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Postal Code</label>
            <input type="number" class="input" value="45962" />
          </div>
          <div class="input__box">
            <label for="" class="input__label">Country</label>
            <input type="text" class="input" value="USA" />
          </div>
        </div>
      </div>
      <button class="button">Save</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.button {
  display: inline-block;
  color: #fff;
  padding: 14px 0;
  width: 190px;
  background-color: #1814f3;
  align-self: self-end;
  border-radius: 15px;
  border: 1px solid transparent;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
  font-size: 18px;
}
.button:hover {
  background-color: transparent;
  border-color: #1814f3;
  color: #1814f3;
}
.input {
  width: 100%;
  height: 50px;
  border-radius: 15px;
  border: 1px solid #dfeaf2;
  color: #718ebf;
  padding: 16px 20px;
  font-size: 15px;
  margin-top: 10px;
  outline: none;
}

.input__label {
  font-size: 16px;
}

li {
  list-style-type: none;
}

.list-link {
  margin-top: 10px;
  display: flex;
  gap: 40px;
}
.link {
  text-decoration: none;
  color: #718ebf;
  transition: color 0.3s ease-in-out;
  font-weight: 600;
  padding: 0 14px;
}
.link:hover {
  color: #1814f3;
}

.link_active {
  color: #1814f3;
  padding-bottom: 10px;
  border-radius: 3px;
  border-bottom: 3px solid #1814f3;
}
.profile {
  background-color: #f5f7fa;
  height: 100%;
  padding: 30px 40px 0;
}

.profile__info {
  display: flex;
  gap: 53px;
}

.info {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(330px, 1fr));
  gap: 24px;
  margin-bottom: 30px;
}

.profile__nav {
  margin-bottom: 65px;
  border-bottom: 1px solid #f5f7fa;
}

.profile__container {
  display: flex;
  padding: 30px;
  flex-direction: column;
  background-color: #fff;
  border-radius: 25px;
  margin-bottom: 30px;
}

.foto {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  overflow: hidden;
}
.foto__container {
  position: relative;
}
.foto__edit {
  position: absolute;
  width: 30px;
  height: 30px;
  top: 85px;
  left: 105px;
  cursor: pointer;
}

@media screen and (max-width: 1024px) {
  .profile__info {
    flex-direction: column;
  }
}

@media screen and (max-width: 768px) {
  .foto__container {
    margin: 0 auto;
  }
  .foto {
    width: 170px;
    height: 170px;
  }
  .foto__edit {
    width: 40px;
    height: 40px;
    top: 112px;
    left: 136px;
  }
  .list-link {
    justify-content: space-between;
    margin-top: 0;
  }
  .profile__nav {
    margin-bottom: 28px;
    border-bottom: 1px #f5f7fa;
  }
  .button {
    width: 100%;
    border-radius: 10px;
    font-size: 15px;
    padding: 11px 0;
  }
  .info {
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 12px;
  }
  .input {
    border-radius: 10px;
  }
  .link {
    font-size: 12px;
    letter-spacing: 0.4px;
    padding: 0 2px 5px 2px;
  }

  .list-link {
    gap: 40px;
    padding-bottom: 5px;
    border-bottom: 1px solid #f5f7fa;
  }
  .profile {
    padding: 25px;
  }
  .profile__info {
    gap: 23px;
  }
  .profile__container {
    padding: 20px;
    border-radius: 15px;
  }
  .input {
    height: 40px;
    font-size: 12px;
  }
  .input__label {
    font-size: 13px;
  }
}
</style>
