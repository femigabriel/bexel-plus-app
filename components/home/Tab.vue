<template>
  <div class="tab">
    <div class="con">
      <table>
        <thead>
          <tr>
            <td>RECIPENT</td>
            <td>TRANSACTION</td>
            <td>DATE</td>
            <td>STATUS</td>
          </tr>
        </thead>

        <tbody>
          <tr class="collapsed">
            <td>
              <div>
                <img src="../../images/avatar-smallsize.svg" alt="avatar" />
                <p>Luka Modric</p>
              </div>
            </td>
            <td>
              <div>
                <span> 1000 CAD </span
                ><span class="material-icons">
                  <i class="las la-caret-right"></i></span
                ><span> 3900 BRL </span>
              </div>
            </td>
            <td>
              <div><span> 2/4/2020 </span></div>
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
                <img src="../../images/avatar-smallsize.svg" alt="avatar" />
                <p>Toni Kross</p>
              </div>
            </td>
            <td>
              <div>
                <span> 1000 CAD </span
                ><span class="material-icons">
                  <i class="las la-caret-right"></i></span
                ><span> 3900 BRL </span>
              </div>
            </td>
            <td>
              <div><span> 2/4/2020 </span></div>
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
                <img src="../../images/avatar-smallsize.svg" alt="avatar" />
                <p>Erin Casimero</p>
              </div>
            </td>
            <td>
              <div>
                <span> 1000 CAD </span
                ><span class="material-icons">
                  <i class="las la-caret-right"></i></span
                ><span> 3900 BRL </span>
              </div>
            </td>
            <td>
              <div><span> 2/4/2020 </span></div>
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
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.tab {
  display: flex;
  justify-content: space-between;
}
.con {
  width: 100%;
  overflow-x: auto;
}

table {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0 10px;
}
tr.collapsed {
  background-color: transparent;
  border-spacing: 0;
}
td {
  border-top: 1px solid #dbe5f4;
  border-bottom: 1px solid #dbe5f4;
  padding: 20px 40px 20px 40px;
  box-sizing: content-box;
}
thead td {
  border-top: none;
  border-bottom: none;
  border: none;
  padding-bottom: 20px;
  font-size: 14px;
  color: #879dad;
}

tbody tr td:first-child {
  padding-left: 1rem;
  border-radius: 6px 0 0 0;
  border-left: 1px solid #dbe5f4;
}
tr td:last-child {
  padding-right: 2px;
  border-radius: 0 6px 0 0;
  border-right: 1px solid #dbe5f4;
}
thead tr td:last-child{
   border: none;
}
tr td div {
  display: flex;
  align-items: center;
}
tr td:first-child img {
  margin-right: 16px;
}
tr td:first-child p {
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 0;
  color: rgba(0, 0, 0, 0.85);
  
}
tr td:last-child div .badge {
  width: 65%;
}
.badge.success {
  border-color: #0fc578;
  background: rgba(15, 197, 120, 0.2);
  color: #129d62;
}
.badge {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 3px 1rem;
  border: 1px solid;
  font-size: 11px;
  font-weight: 700;
  width: fit-content;
  border-radius: 6px;
}
tr td:last-child div button.toggle {
  all: unset;
  padding: 3px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #edf2fc;
  border-radius: 6px;
  border: none;
  margin: 0 15px;
}
.las {
  font-size: 16px;
  margin: 5px;
}
tr td div span {
  color: #879dad;
}
.badge.warning {
  background: rgba(255, 193, 7, 0.2);
  border: 1px solid #fdc008;
  color: #daa917 !important;
}
</style>
