<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Formulario de encuesta</title>
    <style>
      body {
  background: linear-gradient(
    0deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(9, 9, 121, 1) 85%
  );
}

#logo {
  text-align: center;
  margin: 30px auto 0;
  font-size: 100px;
  font-weight: bold;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  color: white;
  text-shadow: 1px 1px 1px #ccc, 1px 1px 1px #ccc, 2px 2px 1px #ccc,
    3px 3px 1px #ccc, 4px 4px 1px #ccc, 5px 5px 1px #ccc, 6px 6px 1px #ccc,
    7px 7px 1px #ccc;
}

#title {
  text-align: center;
  font-size: 36px;
  font-weight: bold;
  color: white;
}

#description {
  text-align: center;
  margin-bottom: 30px;
  font-size: 18px;
  color: white;
}

#survey-form {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
  border: 2px solid #ddd;
  border-radius: 10px;
}

label {
  font-weight: bold;
  display: block;
  margin: 10px 0 10px;
  color: #ddd;
}

input[type="text"],
input[type="email"],
input[type="number"],
textarea,
select {
  display: block;
  width: 96%;
  padding: 10px;
  margin: 0 0 20px 0;
  border-radius: 5px;
  border: 1px solid #ccc;
}

select {
  width: 100%;
}

input[type="text"]:focus,
input[type="email"]:focus,
input[type="number"]:focus,
textarea:focus,
select:focus {
  box-shadow: 0 0 10px 5px #0077cc;
}

input[type="radio"],
input[type="checkbox"] {
  margin-right: 10px;
  margin-bottom: 5px;
}

#submit {
  display: block;
  width: 50%;
  margin: 30px auto 0;
  padding: 10px;
  background-color: #0095ff;
  color: #fff;
  border: none;
  border-radius: 5px;
}

#submit:hover {
  background-color: #005fa3;
}
    </style>
  </head>
  <body>
    <header>
      <h1 id="logo">.NET</h1>
    </header>
    <h1 id="title">Formulario de encuesta</h1>
    <div>
      <p id="description">
        Por favor completa la siguiente encuesta para que podamos mejorar
        nuestro servicio.
      </p>
    </div>
    <form id="survey-form">
      <div class="form-group">
        <label for="name" id="name-label">Nombre completo: </label>
        <input
          type="text"
          id="name"
          name="name"
          required
          placeholder="Ingresa tu nombre completo"
        />
      </div>
      <div class="form-group">
        <label for="email" id="email-label">Correo electrónico: </label>
        <input
          type="email"
          id="email"
          name="email"
          required
          placeholder="Ingresa tu correo electrónico"
        />
      </div>
      <div class="form-group">
        <label for="number" id="number-label">Edad: </label>
        <input
          type="number"
          id="number"
          name="age"
          required
          placeholder="Ingresa tu edad"
          min="18"
          max="99"
        />
      </div>
      <div class="form-group">
        <label for="dropdown" id="dropdown-label">Cómo nos conociste?</label>
        <select id="dropdown" name="dropdown">
          <option value="">Selecciona una opción</option>
          <option value="amigo">Amigo/Familiar</option>
          <option value="internet">Internet</option>
          <option value="publicidad">Publicidad</option>
          <option value="otro">Otro</option>
        </select>
      </div>
      <br />
      <div class="form-group">
        <label id="radio-label">¿Te gustó nuestro servicio?</label>
        <label><input type="radio" name="radio" value="si" required />Si</label>
        <label><input type="radio" name="radio" value="no" />No</label>
      </div>
      <br />
      <div class="form-group">
        <label id="checkbox-label">¿Cuáles de nuestros servicios usaste?</label>
        <label
          ><input
            type="checkbox"
            name="servicio"
            value="internet"
          />Internet</label
        >
        <label
          ><input
            type="checkbox"
            name="servicio"
            value="telefonia"
          />Telefonía</label
        >
        <label
          ><input
            type="checkbox"
            name="servicio"
            value="television"
          />Televisión</label
        >
        <label
          ><input type="checkbox" name="servicio" value="otro" />Otro</label
        >
      </div>
      <br />
      <div class="form-group">
        <label for="comments" id="comments-label"
          >Comentarios adicionales:
        </label>
        <textarea
          id="comments"
          name="comments"
          placeholder="Ingresa tus comentarios"
          rows="5"
        ></textarea>
      </div>
      <div class="form-group">
        <button type="submit" id="submit">Enviar</button>
      </div>
    </form>
  </body>
</html>
