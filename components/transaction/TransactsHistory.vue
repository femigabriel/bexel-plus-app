<template>
  <div class="table-container">
    <div class="table-container">
      <div id="transaction-table">
        <table class="mod-width">
          <colgroup>
            <col style="width: 30%" />
            <col style="width: 20%" />
            <col style="width: 30%" />
            <col style="width: 20%" />
          </colgroup>
          <tbody class="table-alt">
            <tr class="collapsed">
              <td>
                <div>
                  <section>
                    <img
                      src="../../images/avatar-smallsize.svg"
                      alt="avatar"
                      class="avatar-img"
                    /><img
                      src="../../images/brazil-flag.svg"
                      alt=""
                      class="img-attachment"
                    />
                  </section>
                  <p>Luka Modric<small> phillipmango@gmail.com </small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>Jun 6th 2020<small>Last transaction date</small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>
                    <span class="icon-wrap"
                      ><span> 1000 CAD </span
                      ><span class="material-icons">
                        <i class="las la-caret-down"></i> </span
                      ><span> 3900 BRL </span></span
                    ><small>Last transaction amount</small>
                  </p>
                </div>
              </td>
              <td>
                <div>
                  <span class="badge success">COMPLETED </span
                  ><button class="toggle">
                    <span class="material-icons">
                      <i class="las la-caret-down"></i
                    ></span>
                  </button>
                </div>
              </td>
            </tr>
            <tr class="collapsed">
              <td>
                <div>
                  <section>
                    <img
                      src="../../images/avatar-smallsize.svg"
                      alt="avatar"
                      class="avatar-img"
                    /><img
                      src="../../images/brazil-flag.svg"
                      alt=""
                      class="img-attachment"
                    />
                  </section>
                  <p>Toni Kross<small> phillipmango@gmail.com </small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>Jun 1st 2020<small>Last transaction date</small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>
                    <span class="icon-wrap"
                      ><span> 1000 CAD </span
                      ><span class="material-icons">
                        <i class="las la-caret-right"></i> </span
                      ><span> 3900 BRL </span></span
                    ><small>Last transaction amount</small>
                  </p>
                </div>
              </td>
              <td>
                <div>
                  <span class="badge success">COMPLETED </span
                  ><button class="toggle">
                    <span class="material-icons">
                      <i class="las la-caret-down"></i>
                    </span>
                  </button>
                </div>
              </td>
            </tr>
            <tr class="collapsed">
              <td>
                <div>
                  <section>
                    <img
                      src="../../images/avatar-smallsize.svg"
                      alt="avatar"
                      class="avatar-img"
                    /><img
                      src="../../images/brazil-flag.svg"
                      alt=""
                      class="img-attachment"
                    />
                  </section>
                  <p>Erin Casemiro<small> ericculhane@gmail.com </small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>May 17th 2020<small>Last transaction date</small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>
                    <span class="icon-wrap"
                      ><span> 1000 CAD </span
                      ><span class="material-icons">
                        <i class="las la-caret-down"></i> </span
                      ><span> 3900 BRL </span></span
                    ><small>Last transaction amount</small>
                  </p>
                </div>
              </td>
              <td>
                <div>
                  <span class="badge warning">PENDING </span
                  ><button class="toggle">
                    <span class="material-icons">
                      <i class="las la-caret-down"></i>
                    </span>
                  </button>
                </div>
              </td>
            </tr>
            <tr class="collapsed">
              <td>
                <div>
                  <section>
                    <img
                      src="../../images/avatar-smallsize.svg"
                      alt="avatar"
                      class="avatar-img"
                    /><img
                      src="../../images/brazil-flag.svg"
                      alt=""
                      class="img-attachment"
                    />
                  </section>
                  <p>Karim Benzema<small> ericculhane@gmail.com </small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>May 17th 2020<small>Last transaction date</small></p>
                </div>
              </td>
              <td>
                <div>
                  <p>
                    <span class="icon-wrap"
                      ><span> 1000 CAD </span
                      ><span class="material-icons">
                        <i class="las la-caret-right"></i> </span
                      ><span> 3900 BRL </span></span
                    ><small>Last transaction amount</small>
                  </p>
                </div>
              </td>
              <td>
                <div>
                  <span class="badge danger">CANCELLED </span
                  ><button class="toggle">
                    <span class="material-icons">
                      <i class="las la-caret-down"></i>
                    </span>
                  </button>
                </div>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.table-container {
  width: 100%;
  overflow-x: auto;
}
#transaction-table {
  width: 100%;
  overflow-x: auto;
}
table.mod-width {
  width: 99%;
  margin: auto;
}
#transaction-table table {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0 10px;
}

tr.collapsed {
  background-color: #fff;
}
tr td:first-child {
  box-shadow: 0 -2px 7px -5px rgb(169 181 192 / 20%),
    0 5px 7px -5px rgb(169 181 192 / 20%),
    -5px 0 7px -5px rgb(169 181 192 / 20%);
  padding-left: 1.4rem;
}
tr td div {
  display: flex;
  align-items: center;
}
tr td div section {
  position: relative;
  display: flex;
  justify-content: center;
  padding-bottom: 9px;
}
tr td div .avatar-img {
  width: 40px;
  height: 40px;
}
tr td:first-child img {
  margin-right: 1rem;
}
tr td div section .img-attachment {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 16px;
  margin: 0 auto;
  height: 19px;
  width: 19px;
}
td div p {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-bottom: 0;
  font-weight: 500;
  color: #4a4b65;
  width: 12em;
  font-size: 16px;
}
tr td:first-child p {
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 0;
}
tr td div p small {
  display: inherit;
  color: #879dad;
  font-weight: 400;
}
small {
  font-size: 12.8px;
}
.las {
  font-size: 16px;
}
.badge.danger {
  background: rgba(243, 67, 53, 0.2);
  border: 1px solid #f34335;
  color: #d63629;
}
</style>
