<template>
  <!-- Button trigger modal -->
  <button
    type="button"
    class="btn btn-primary"
    data-bs-toggle="modal"
    data-bs-target="#exampleModal"
  >
    crear estudiante
  </button>
  

  <!-- Modal -->
  <div
    class="modal fade"
    id="exampleModal"
    tabindex="-1"
    aria-labelledby="exampleModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="exampleModalLabel">
            Crear estudiante
          </h1>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <form id="formnew" enctype="multipart/form-data">
            <div class="mb-2">
              <label for="message-text" class="col-form-label text-black"
                >DNI:</label
              >
              <input type="text" class="form-control" id="recipient-name" />
            </div>
            <div class="mb-2">
              <label for="categori" class="col-form-label text-black"
                >First name:
              </label>
              <input type="text" class="form-control" id="categori" />
            </div>
            <div class="mb-2">
              <label for="code" class="col-form-label text-black"
                >Family name:</label
              >
              <input type="text" class="form-control" id="code" />
            </div>
            <div class="mb-2">
              <label for="price" class="col-form-label text-black"
                >Email:
              </label>
              <input type="text" class="form-control" id="price" />
            </div>
            <div class="mb-2">
              <label for="stock" class="col-form-label text-black">Age:</label>
              <input type="text" class="form-control" id="stock" />
            </div>
            <div class="mb-2">
              <label for="description" class="col-form-label text-black"
                >Phone number:
              </label>
              <input type="text" class="form-control" id="description" />
            </div>
          </form>
        </div>
        <div class="modal-footer">
          <button
            type="button"
            class="btn btn-secondary"
            data-bs-dismiss="modal"
          >
            cerrar
          </button>
          <button type="button" class="btn btn-primary">guardar</button>
        </div>
      </div>
    </div>
  </div>

  <div id="container_home">
    <div id="welcome">
      <div id="welcome2">
        <input
          name="buscar estudiante"
          class="em"
          type="text"
          id="buscar"
          placeholder="Buscar estudiante"
        />
      </div>

      <aside id="lado">
        <ul class="nav flex-column">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled">link</a>
          </li>
        </ul>
      </aside>
    </div>

    <div id="home">
      <div class="section">
        <section id="seccion">
          <table class="table">
            <thead>
             
                <tr>
      <th scope="col"><b>dni</b></th>
      <th scope="col"><b>First</b></th>
      <th scope="col"><b>family name</b></th>
      <th scope="col"><b>email</b></th>
      <th scope="col"><b>age</b></th>
      <th scope="col"><b>phone</b></th>
      <th scope="col"><b>address</b></th>
    </tr>
                
            </thead>
            
            <tbody class="table-group-divider">
              <tr>
                <th scope="row">1117550550</th>
                <td>karolina</td>
                <td>segura</td>
                <td>ksegura1@misena.edu.co</td>
                <td>1998</td>
                <td>3142613646</td>
                <td>acacias</td>
                <td>
                  <a
                    name=""
                    id="edit"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleditar"
                    >editar</a
                  >
                  <a
                    name=""
                    id="elimi"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleliminar"
                    >eliminar</a
                  >
                </td>
              </tr>
              <tr>
                <th scope="row">1006585292</th>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>jacob@gmail.com</td>
                <td>2004</td>
                <td>3112220542</td>
                <td>cunduy</td>
                <td>
                  <a
                    name=""
                    id="edit"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleditar"
                    >editar</a
                  >
                  <a
                    name=""
                    id="elimi"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleliminar"
                    >eliminar</a
                  >
                </td>
              </tr>
              <tr>
                <th scope="row">12345667</th>
                <td>Larry</td>
                <td>perdomo</td>
                <td>larry@gmail.com</td>
                <td>2001</td>
                <td>3114567897</td>
                <td>americas</td>
                <td>
                  <a
                    name=""
                    id="edit"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleditar"
                    >editar</a
                  >
                  <a
                    name=""
                    id="elimi"
                    class="btn btn-primary"
                    data-bs-toggle="modal"
                    data-bs-target="#modaleliminar"
                    >eliminar</a
                  >
                </td>
              </tr>
            </tbody>
          </table>
        </section>
      </div>
      <router-view> </router-view>
    </div>
  </div>
  <!-- ---------------modales-------------------- -->
  <!-- Modal -->
  <div
    class="modal fade"
    id="modaleditar"
    data-bs-backdrop="static"
    data-bs-keyboard="false"
    tabindex="-1"
    aria-labelledby="staticBackdropLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="staticBackdropLabel">
            Editar estudiante
          </h1>
          
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <form id="formnew" enctype="multipart/form-data">
            <div class="mb-2">
              <label for="message-text" class="col-form-label text-black"
                >DNI:</label
              >
              <input type="text" class="form-control" id="recipient-name" />
            </div>
            <div class="mb-2">
              <label for="categori" class="col-form-label text-black"
                >First name:
              </label>
              <input type="text" class="form-control" id="categori" />
            </div>
            <div class="mb-2">
              <label for="code" class="col-form-label text-black"
                >Family name:</label
              >
              <input type="text" class="form-control" id="code" />
            </div>
            <div class="mb-2">
              <label for="price" class="col-form-label text-black"
                >Email:
              </label>
              <input type="text" class="form-control" id="price" />
            </div>
            <div class="mb-2">
              <label for="stock" class="col-form-label text-black">Age:</label>
              <input type="text" class="form-control" id="stock" />
            </div>
            <div class="mb-2">
              <label for="description" class="col-form-label text-black"
                >Phone number:
              </label>
              <input type="text" class="form-control" id="description" />
            </div>
          </form>
        </div>
        <div class="modal-footer">
          <button
            type="button"
            class="btn btn-secondary"
            data-bs-dismiss="modal"
          >
            cerrar
          </button>
          <button type="button" class="btn btn-primary">guardar</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Modal2 -->
  <div
    class="modal fade"
    id="modaleliminar"
    data-bs-backdrop="static"
    data-bs-keyboard="false"
    tabindex="-1"
    aria-labelledby="staticBackdropLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="staticBackdropLabel">
            Eliminar estudiante
          </h1>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">Esta seguro de eliminar estudiante</div>
        <div class="modal-footer">
          <button
            type="button"
            class="btn btn-secondary"
            data-bs-dismiss="modal"
          >
            Cerrar
          </button>
          <button type="button" class="btn btn-primary">Eliminar</button>
        </div>
      </div>
    </div>
  </div>
  
</template>
<style scoped>
@import url(../assets/teacher.css);
</style>

<script>
export default {
  data() {
    return {};
  },
  mounted() {},

  methods: {},
};
</script>
