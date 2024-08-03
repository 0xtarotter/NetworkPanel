<template>
  <el-container>
    <el-header class="header">
      <div style="margin-top: 15px;">
        <div style="width: fit-content;float: left;">
          <div class="icon">
            <svg t="1702892592527" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"
              p-id="4460" data-spm-anchor-id="a313x.search_index.0.i9.1e343a81LSbmza">
              <path
                d="M568.96 459.242667l144-189.205334A382.208 382.208 0 0 0 512 213.333333c-212.074667 0-384 171.925333-384 384a382.293333 382.293333 0 0 0 93.397333 251.008l-64.554666 55.808A467.584 467.584 0 0 1 42.666667 597.333333C42.666667 338.133333 252.8 128 512 128c93.098667 0 179.861333 27.093333 252.842667 73.856l75.882666-99.690667 67.541334 51.413334-273.28 359.04a149.333333 149.333333 0 1 1-66.048-53.376z m266.453333-69.056l54.357334-71.424A467.242667 467.242667 0 0 1 981.333333 597.333333c0 113.706667-40.64 221.226667-113.237333 305.728l-64.725333-55.616A382.272 382.272 0 0 0 896 597.333333c0-76.288-22.250667-147.370667-60.586667-207.146666zM512 661.333333a64 64 0 1 0 0-128 64 64 0 0 0 0 128z"
                fill="#ffffff" p-id="4461"></path>
            </svg>
          </div>
          <span class="title"> Cesu.Wang </span>
        </div>
        <div style="float: right;margin-top: 5px;">
          <el-button class="home" @click="aboutVisible=true" round>关于</el-button>
        </div>
        <div v-if="isAndroid" style="float: right;margin-top: 5px;margin-right: 5px;">
          <el-button class="home" @click="downLoadAPPTableVisible=true" round>APP</el-button>
        </div>
      </div>
    </el-header>
    <el-main>
      <MainUI :isVisible="isVisible" />
      <br>
      <IPinfoUI :isVisible="isVisible" />
    </el-main>
    <div style="height: fit-content;padding-bottom: 10px;">
      <div style="width: fit-content;margin-left: auto;margin-right: auto;">
        <el-link type="info" @click='open("https://39MI.COM/")' target="_blank">
		
	<center>
  <a href="https://39mi.com" target="_blank" style="text-decoration:none;">    
	<img src="data:image/svg+xml;base64,PHN2ZyBjbGFzcz0iaWNvbiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB3aWR0aD0iNDUiIGhlaWdodD0iNDUiPjxwYXRoIGQ9Ik01MTEuMTI1IDYzLjU2MmMyNDcuMDA3IDAgNDQ3LjI0OCAyMDAuMjQxIDQ0Ny4yNDggNDQ3LjI1IDAgMjQ3LjAxLTIwMC4yNDEgNDQ3LjI1LTQ0Ny4yNDggNDQ3LjI1LTI0Ny4wMSAwLTQ0Ny4yNTEtMjAwLjI0LTQ0Ny4yNTEtNDQ3LjI1IDAtMjQ3LjAwOSAyMDAuMjQtNDQ3LjI1IDQ0Ny4yNTEtNDQ3LjI1eiIgZmlsbD0iI0VFRSIvPjxwYXRoIGQ9Ik03MTEuNjc3IDkwNy44NzJjLTU5LjIxMyAyOC45MzYtMTI1LjczNyA0NS4yMi0xOTYuMDgxIDQ1LjIyLTg2LjcyNyAwLTE2Ny42MzUtMjQuNzYtMjM2LjE4OC02Ny40OSA3OS4yMzctMjAuNDY3IDE1NS44MjUtMTIuMjE0IDE3My4yMzQtNDguMTY2IDQwLjgxNi04MC4zMzcgMjAuNDE4LTExMC44Mi0zNi45NzQtMTIxLjE2OC03OC4wMy0yMC45NTItOTguOTcyLTU0LjgyOC04OS4xODQtMjUxLjk3OCAxOS4zMjUtMTA0LjQ0NCA0LjEtMzAzLjQxNCAyNDUuMDM2LTI2Ny40MDMgMjQ1Ljc0NyAzNi43NDYgMTcyLjIwNiAyNDYuODEgNjkuMjcyIDUwMC41NzQtNTIuODIyIDEzMC4yMzEgMjYuMDAzIDE4OC43MDYgNzAuODg1IDIxMC40MTF6IiBmaWxsPSIjRkZGIi8+PC9zdmc+" />
  <br />
<img data-v-b2352fe5="" src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjE5My44MzYgNDk5LjIzNiAxMDYzLjg0MiAxNjUuOTAxIj48cGF0aCBkPSJNMjUxLjEzIDU3MC43Yy0uNDktMS0xLjEzLTIuMjgtMy40NC0zLjQzLTIuMzEtMS4xNS00LjMyLTIuMS04LjEzLTIuMzItMy44LS4yMS04Ljc2LjM0LTEwLjkxIDEuMjQtMi4xNS45MS0xLjk2IDIuNTguMTUgMy4zIDIuMTEuNzIgNi45LS4wMyAxMC40LjMgMy40OS4zNCA0Ljg3Ljg5IDcuMDYgMS4zOCAyLjE5LjUgMi45MiAxLjIgMy45IDEuMS45Ny0uMDkgMS40Ni0uNTcuOTctMS41NyIgc3Ryb2tlPSIjMDAwIi8+PHBhdGggZD0iTTIwNy40OCA1NzguMDNjLTEuMzIgMS40OS0zIDMuOTgtNC44NSA4LjM5LTEuODUgNC40Mi0zLjI5IDcuOC00LjQgMTMuNjctMS4xMiA1Ljg3LTEuNzUgMTAuMDEtMS4xOCAxNS42OC41NyA1LjY4IDEuNTUgOC4zOSA0LjAyIDEyLjcxIDIuNDYgNC4zMiA0LjUxIDYuMjMgOC4zMiA4LjkxIDMuODIgMi42NyA2LjI2IDMuNzggMTAuNzQgNC40NiA0LjQ4LjY4IDcuMTYuNjEgMTEuNjUtMS4wNiA0LjQ5LTEuNjggNi44Ny0zLjI4IDEwLjgxLTcuMzMgMy45NC00LjA2IDUuODgtNi43OCA4Ljg4LTEyLjk1IDMuMDEtNi4xOCA0LjI4LTEwLjA5IDYuMTUtMTcuOTIgMS44OC03Ljg0IDIuNTMtMTIuNTggMy4yMy0yMS4yNi43MS04LjY4LjYzLTEzLjcuMy0yMi4xNXMtLjk3LTEyLjkyLTEuOTQtMjAuMTFjLS45Ny03LjE4LTEuNzQtMTAuNTktMi45Mi0xNS44LTEuMTktNS4yMS0xLjY1LTcuNzQtMy0xMC4yNS0xLjM0LTIuNTEtMi41OC0yLjkyLTMuNzItMi4zMi0xLjE0LjYtMS44OSAxLjg1LTEuOTggNS4zMi0uMDkgMy40Ny40MyA2LjMyIDEuNTMgMTIuMDIgMS4xMSA1LjcxIDEuOTMgOS41MSA0IDE2LjUyIDIuMDggNy4wMSAzLjU0IDExLjI4IDYuMzcgMTguNTQgMi44NCA3LjI1IDQuNDEgMTAuOTggNy44MSAxNy43MyAzLjQxIDYuNzUgNS40OSAxMC4yOCA5LjIyIDE2LjAyIDMuNzIgNS43NSA1LjY5IDguMyA5LjQgMTIuNyAzLjcyIDQuNDEgNS42MSA2LjM5IDkuMTggOS4zMyAzLjU3IDIuOTUgNS4yNCA0LjEgOC42NyA1LjM5IDMuNDMgMS4yOSA1LjM2IDEuNTQgOC41IDEuMDYgMy4xNS0uNDggNC42Ni0xLjQgNy4yMi0zLjQ2IDIuNTctMi4wNiAzLjcyLTMuNjcgNS42LTYuODQgMS44OC0zLjE2IDIuNS01LjM1IDMuNzktOSAxLjI5LTMuNjQgMi4xNi01Ljk4IDIuNjctOS4yMi41Mi0zLjI0LjQzLTUuMi0uMS02Ljk4LS41My0xLjc4LTEuNTUtMi4yOC0yLjUzLTEuOS0uOTkuMzctMi4wMiAxLjQ2LTIuNDIgMy44LS4zOSAyLjM0LS42MSA0LjU0LjQ2IDcuOTFzMi4yNSA1LjY5IDQuODggOC45M2MyLjYyIDMuMjUgNC40MyA0Ljg2IDguMjUgNy4yOSAzLjgyIDIuNDIgNi4yNyAzLjQ0IDEwLjgzIDQuODQgNC41NiAxLjQgNy4yOCAxLjk1IDExLjk2IDIuMTcgNC42OS4yMSA3LjI0LS4wOSAxMS40OC0xLjExIDQuMjQtMS4wMyA2LjUyLTEuODUgOS43Mi00LjAzIDMuMi0yLjE4IDQuNy0zLjc0IDYuMjctNi44OCAxLjU3LTMuMTUgMi4wOS01LjQgMS41OS04Ljg2LS40OS0zLjQ2LTEuMy01LjQ2LTQuMDctOC40NS0yLjc3LTIuOTgtNS4wNy00LjY0LTkuNzctNi40OS00LjcxLTEuODUtOC0yLjM2LTEzLjc0LTIuNzYtNS43NC0uNC05LjMtLjE0LTE0Ljk3Ljc0LTUuNjcuODctOS4wMiAxLjY1LTEzLjM5IDMuNjMtNC4zNiAxLjk5LTYuMzYgMy41OS04LjQxIDYuMjgtMi4wNSAyLjY5LTEuODcgNC44MS0xLjgzIDcuMTkuMDQgMi4zOCAxLjMxIDMuODYgMi4wMiA0LjcyLjcuODYgMS4zMi40OCAxLjUtLjQ0LjE4LS45My0uNzktMi4yOS0uNi00LjE4LjE5LTEuODgtLjE0LTMuMDUgMS41Ny01LjI1IDEuNy0yLjE5IDMuMDQtMy44NyA2Ljk1LTUuNzQgMy45MS0xLjg4IDcuMjEtMi43NiAxMi42LTMuNjEgNS4zOS0uODYgOC45Mi0xLjA5IDE0LjM2LS42NiA1LjQ0LjQ0IDguNTggMS4wNiAxMi44MyAyLjgyIDQuMjUgMS43NyA2LjE0IDMuNDcgOC40MiA2IDIuMjggMi41NCAyLjYyIDMuOTkgMi45NyA2LjY4LjM0IDIuNjktLjAxIDQuMjctMS4yNSA2Ljc3cy0yLjI1IDMuODQtNC45NSA1Ljc0Yy0yLjcxIDEuODktNC43NCAyLjc3LTguNTcgMy43NS0zLjg0Ljk3LTYuMjQgMS4zMS0xMC42IDEuMTMtNC4zNS0uMTktNi45NS0uNzItMTEuMTgtMi4wNy00LjIyLTEuMzQtNi41Ni0yLjM2LTkuOTMtNC42Ny0zLjM4LTIuMzEtNC45MS0zLjktNi45Mi02Ljg4LTIuMDItMi45OS0yLjM0LTUuMTUtMy4xNS04LjA2cy0uNDgtNC41My0uOS02LjQ5Yy0uNDMtMS45NS0uNzEtMi45MS0xLjIzLTMuMjktLjUzLS4zNy0uODYtLjEtMS40IDEuNDEtLjU1IDEuNTEtLjY5IDMuMTQtMS4zNSA2LjEzLS42NSAyLjk5LS44NyA1LjM5LTEuOTMgOC44MS0xLjA2IDMuNDItMS43NCA1LjQ3LTMuMzUgOC4yOS0xLjYxIDIuODMtMi42OCA0LjA3LTQuNjggNS44Mi0yLjAxIDEuNzQtMi45IDIuNDEtNS4zNCAyLjkxcy0zLjg2LjU1LTYuODUtLjQyYy0yLjk5LS45OC00LjY2LTEuODItOC4xLTQuNDctMy40NS0yLjY0LTUuNDItNC41My05LjEzLTguNzQtMy43Mi00LjIyLTUuNzItNi43MS05LjQ1LTEyLjM0LTMuNzItNS42Mi01LjgxLTkuMTItOS4xOC0xNS44LTMuMzctNi42Ny00LjkzLTEwLjM4LTcuNjYtMTcuNTktMi43My03LjIxLTQuMTItMTEuNDktNS45Ny0xOC40Ni0xLjg2LTYuOTgtMi40Ny0xMC43OS0zLjMyLTE2LjQtLjg1LTUuNjItLjU4LTguNDQtLjk0LTExLjY4LS4zNy0zLjIzLS44LTQuMTctLjg5LTQuNTEtLjA4LS4zNC0uMzMuMzEuNDUgMi44Ljc4IDIuNDkgMi4xIDQuNjIgMy40NiA5LjY2IDEuMzYgNS4wMyAyLjI1IDguNDMgMy4zMyAxNS41MiAxLjA4IDcuMDggMS43MiAxMS41NCAyLjA4IDE5LjkxLjM1IDguMzcuNDIgMTMuMzYtLjMxIDIxLjk0LS43MiA4LjU4LTEuNDEgMTMuMjgtMy4zMiAyMC45Ni0xLjkyIDcuNjgtMy4yNSAxMS41MS02LjI0IDE3LjQzLTMgNS45Mi00Ljk3IDguNDUtOC43MiAxMi4xOS0zLjc1IDMuNzQtNS45NiA1LjA0LTEwLjAzIDYuNTEtNC4wNyAxLjQ2LTYuMzIgMS40My0xMC4zMS44MS0zLjk5LS42MS02LjE4LTEuNTEtOS42NC0zLjg5LTMuNDYtMi4zNy01LjM5LTQuMDQtNy42NC03Ljk4LTIuMjYtMy45My0zLjE2LTYuMzctMy42NC0xMS42OS0uNDgtNS4zMy4xMy05LjMxIDEuMjMtMTQuOTMgMS4xLTUuNjIgMi42LTguODQgNC4yOC0xMy4xNiAxLjY5LTQuMzIgMy42Ny02LjU4IDQuMTMtOC40Ni40Ny0xLjg4LS40Ni0yLjQ0LTEuNzktLjk1TTQwMSA1ODMuNTdjLS4yMSAxLjA4LS4wMiAyLjM1LjcxIDQuNjMuNzIgMi4yOCAxLjUyIDMuNzkgMi45IDYuNzYgMS4zOSAyLjk3IDIuMzkgNC45IDQuMDIgOC4wOSAxLjYzIDMuMTkgMi4zNiA1LjMyIDQuMTMgNy44OCAxLjc3IDIuNTYgMi43NyAzLjgzIDQuNzEgNC45MSAxLjkzIDEuMDcgMy4wOSAxLjIgNC45Ny40N3MyLjk2LTEuNjQgNC40MS00LjExYzEuNDUtMi40NyAxLjc3LTQuNzUgMi44My04LjI2czEuNDUtNS45NiAyLjQ3LTkuMzFjMS4wMy0zLjM1IDEuNjItNS4xMiAyLjY3LTcuNDUgMS4wNS0yLjM0IDEuMjktMy4zNSAyLjU3LTQuMjMgMS4yOS0uODkgMS45OS0uNzQgMy44Ni0uMiAxLjg2LjU1IDMuMDQgMS4zNSA1LjQ5IDIuOTIgMi40NSAxLjU4IDMuOTggMi43OCA2Ljc2IDQuOTcgMi43OCAyLjIgNC40MiAzLjc1IDcuMTYgNi4wMiAyLjc0IDIuMjcgMy45MiAzLjc2IDYuNTMgNS4zMyAyLjYyIDEuNTcgNC4wNCAyLjExIDYuNTQgMi41MiAyLjUxLjQgMy42NC4xOSA1Ljk4LS41MSAyLjMzLS43IDMuNS0xLjQ4IDUuNy0zIDIuMi0xLjUzIDMuMjEtMi42MSA1LjI4LTQuNjMgMi4wNy0yLjAzIDMuMTUtMy41NCA1LjA5LTUuNDkgMS45NC0xLjk2IDIuNzctMy4wNSA0LjYxLTQuMyAxLjg0LTEuMjQgMi42MS0xLjc3IDQuNTgtMS45MyAxLjk3LS4xNSAyLjkxLjE3IDUuMjcgMS4xNCAyLjM1Ljk4IDMuNyAxLjkxIDYuNSAzLjc2IDIuODEgMS44NCA0LjQgMy4yIDcuNTMgNS40NiAzLjEyIDIuMjYgNC43IDMuNTkgOC4xMiA1LjgyIDMuNDIgMi4yMyA1LjI5IDMuNTYgOC45OCA1LjMxIDMuNyAxLjc2IDUuNzkgMi42NiA5LjQ5IDMuNDcgMy43MS44IDUuNDkuODYgOS4wNC41NiAzLjU1LS4yOSA1LjM4LS43IDguNjktMi4wMyAzLjMyLTEuMzMgNS4xMi0yLjE0IDcuOS00LjYgMi43OC0yLjQ2IDMuODEtNC4yOCA2LTcuNjkgMi4xOC0zLjQgMy4xOS01LjY2IDQuOTEtOS4zNCAxLjcyLTMuNjggMi44Ni01LjgxIDMuNjktOS4wNy44My0zLjI3Ljk0LTUuMjIuNDYtNy4yNS0uNDgtMi4wMy0xLjUzLTIuODItMi44NS0yLjkxLTEuMzMtLjA4LTIuNDcuNTktMy43NyAyLjQ5LTEuMjkgMS45MS0yLjE1IDMuNzUtMi43IDcuMDYtLjU0IDMuMzEtLjUxIDUuNjQtLjA0IDkuNS40NyAzLjg1IDEgNi4xMiAyLjM5IDkuNzggMS40IDMuNjUgMi4zOSA1LjQgNC41OSA4LjQ4IDIuMiAzLjA4IDMuNjMgNC41OSA2LjQyIDYuOTEgMi43OSAyLjMyIDQuNSAzLjUyIDcuNTMgNC43IDMuMDQgMS4xNyA0LjczIDEuNDEgNy42NCAxLjE4IDIuOTEtLjIzIDQuNi0uNzUgNi45MS0yLjM0IDIuMzEtMS41OCAzLjQ0LTIuOTMgNC42NC01LjYgMS4yLTIuNjYgMS4zMi00LjY0IDEuMzUtNy43My4wMy0zLjA4LS40Mi01LTEuMTgtNy42OC0uNzctMi42Ny0xLjU4LTQuMDgtMi42NS01LjctMS4wNy0xLjYxLTEuOTktMi4wNy0yLjcyLTIuMzgtLjc0LS4zMS0xLjIxLS4wMS0uOTYuODIuMjQuODMuNTYgMS44NCAyLjE4IDMuMzQgMS42MiAxLjUgMy4xIDIuNTMgNS45MyA0LjE1IDIuODMgMS42MyA0Ljc2IDIuMzcgOC4yMyAzLjk3IDMuNDcgMS42IDUuNTkgMi42NiA5LjEzIDQuMDQgMy41NCAxLjM5IDUuMTMgMi4xIDguNTcgMi44NyAzLjQ0Ljc3IDUuNDIgMS4wOSA4LjY0Ljk4IDMuMjItLjExIDQuNzItLjQzIDcuNDUtMS41MiAyLjczLTEuMSA0LjAyLTEuOTggNi4yMS0zLjk0IDIuMTktMS45NiAzLjIxLTMuMzUgNC43Mi01Ljg4IDEuNTItMi41NCAyLjE0LTQuMjEgMi44NC02LjgxLjcxLTIuNi43NS00LjI1LjY5LTYuMi0uMDYtMS45Ni0uOC0zLjA2LS45OS0zLjU3LS4yLS41LS40Ni0uMDguMDEgMS4wNS40NiAxLjE0Ljg1IDIuNDIgMi4zMSA0LjYyIDEuNDYgMi4xOSAyLjc1IDMuNTggNSA2LjM2IDIuMjQgMi43OCAzLjg3IDQuNzQgNi4yNCA3LjU0czMuNDggNC41MSA1LjYxIDYuNDZjMi4xMyAxLjk2IDMuODEgMi45IDUuMDYgMy4zMiAxLjI1LjQyIDEuNiAwIDEuMi0xLjIyLS40LTEuMjEtMS41My0yLjU5LTMuMjItNC44NS0xLjY5LTIuMjctMy4wNC0zLjYzLTUuMjQtNi40N3MtMy43LTQuODUtNS43Ni03Ljc0Yy0yLjA2LTIuODktMi43NC00LjYxLTQuNTUtNi43MS0xLjgxLTIuMS0yLjg1LTMuMS00LjUyLTMuOC0xLjY4LS43LTIuNzMtLjU5LTMuODUuMy0xLjEzLjg5LTEuMjQgMi4yMy0xLjc4IDQuMTUtLjU1IDEuOTEtLjMxIDMuMi0uOTUgNS40NC0uNjUgMi4yNC0xLjExIDMuNTgtMi4yOCA1Ljc0LTEuMTcgMi4xNi0xLjkgMy4zOS0zLjU2IDUuMDYtMS42NyAxLjY3LTIuNjIgMi4zNy00Ljc3IDMuMjktMi4xNi45MS0zLjI5IDEuMTYtNi4wMyAxLjI4LTIuNzQuMTMtNC41MyAwLTcuNjUtLjY2LTMuMTMtLjY2LTQuNjQtMS4yNy03Ljk2LTIuNjYtMy4zMS0xLjM4LTUuNDMtMi40Ny04LjYyLTQuMjgtMy4yLTEuOC00LjcyLTIuOTktNy4zNC00Ljc0LTIuNjEtMS43NS0zLjcxLTMtNS43Mi00cy0zLjA4LTEuMTktNC4zMy0xYy0xLjI1LjE5LTEuNjYuODItMS45MiAxLjkzLS4yNyAxLjEuMTIgMS44NS41OSAzLjYxLjQ4IDEuNzUgMS4yIDIuODMgMS43NyA1LjE1LjU3IDIuMzIuOTUgMy45NSAxLjA5IDYuNDQuMTQgMi40OS4yNSA0LjAyLS4zOSA2LS42NCAxLjk5LTEuMjggMi44NC0yLjgyIDMuOTMtMS41NSAxLjA5LTIuNzQgMS40My00Ljg5IDEuNTUtMi4xNS4xMS0zLjM2LS4wNC01Ljg1LS45OS0yLjQ5LS45Ni00LjExLTEuODItNi42MS0zLjc5LTIuNDktMS45Ny0zLjg5LTMuMzItNS44Ni02LjA2LTEuOTgtMi43NC0yLjg5LTQuMzQtNC4wMi03LjY0LTEuMTMtMy4yOS0xLjQ3LTUuNDItMS42Mi04Ljg1LS4xNC0zLjQzLjQ1LTUuMzkuOS04LjMuNDYtMi45MSAxLjA4LTQuNDMgMS4zNy02LjI2LjI4LTEuODMuMTUtMi42NS4wNS0yLjg4LS4xLS4yMi0uMTYuMi0uNTQgMS43Ni0uMzggMS41NS0uNSAzLjA5LTEuMzUgNi4wMy0uODYgMi45NC0xLjQ1IDUuMTYtMi45NCA4LjY4LTEuNSAzLjUzLTIuNTYgNS43OC00LjU1IDguOTQtMS45OSAzLjE2LTIuOTQgNC43MS01LjM5IDYuODctMi40NSAyLjE1LTMuOTUgMi43NC02Ljg1IDMuODktMi45IDEuMTYtNC41MiAxLjU3LTcuNjQgMS44Ny0zLjEyLjI5LTQuNjQuMzEtNy45OC0uNC0zLjM1LS43LTUuMjktMS40OC04Ljc0LTMuMTMtMy40Ni0xLjY1LTUuMjgtMi45LTguNTQtNS4xMS0zLjI3LTIuMi00Ljc2LTMuNTUtNy44MS01LjkyLTMuMDQtMi4zNi00LjQ5LTMuOC03LjQxLTUuODktMi45My0yLjA4LTQuMzEtMy40Mi03LjItNC41Mi0yLjktMS4wOS00LjUxLTEuMTgtNy4yNi0uOTQtMi43Ni4yNC00LjA1LjgzLTYuNTEgMi4xNC0yLjQ2IDEuMzItMy41OCAyLjQ2LTUuOCA0LjQ0LTIuMjIgMS45OS0zLjM0IDMuNDctNS4zIDUuNDktMS45NSAyLjAyLTIuNzYgMy4wNy00LjQ4IDQuNi0xLjczIDEuNTMtMi41MiAyLjMyLTQuMTQgMy4wMy0xLjYyLjcxLTIuMjEuOTQtMy45OC41Mi0xLjc4LS40MS0yLjY3LTEuMTEtNC44OS0yLjU5LTIuMjMtMS40OS0zLjU2LTIuNjQtNi4yMi00Ljg0LTIuNjctMi4xOS00LjI5LTMuODEtNy4xMy02LjE0LTIuODMtMi4zMy00LjIyLTMuODQtNy4wNi01LjUxLTIuODQtMS42OC00LjQ0LTIuNTMtNy4xNC0yLjg3LTIuNy0uMzQtNC4xMi0uMDgtNi4zNCAxLjE3LTIuMjEgMS4yNC0zLjE5IDIuNDItNC43MyA1LjA2LTEuNTUgMi42My0xLjgzIDQuNjYtMi45OCA4LjEzLTEuMTYgMy40OC0xLjcxIDUuODctMi43OSA5LjI1cy0xLjgyIDUuMzUtMi42MSA3LjY0Yy0uNzkgMi4yOS0uNzQgMy4yLTEuMzUgMy44Mi0uNjIuNjItLjg0LjM5LTEuNzItLjczLS44Ny0xLjExLTEuMzItMi4zOS0yLjY2LTQuODUtMS4zNC0yLjQ2LTIuNDktNC4zNC00LjA2LTcuNDUtMS41Ni0zLjExLTIuMzUtNS4xNi0zLjc2LTguMDctMS40MS0yLjkyLTIuMDUtNC41LTMuMjktNi41Mi0xLjI0LTIuMDItMS45OC0zLjAyLTIuOTItMy41OHMtMS41Ni0uMy0xLjc4Ljc4TTY2My4yOCA1MjUuOTljLS4xLjY2LjczIDEuODIgMS4zOSAxLjkzLjY1LjExIDEuOC0uNzIgMS45LTEuMzguMTEtLjY2LS43My0xLjgxLTEuMzgtMS45Mi0uNjYtLjExLTEuODEuNzEtMS45MSAxLjM3TTcwNy41MSA1NzUuNjljLjY0LjM1IDEuMi0uMDUgMi4zMS0uMDEgMS4xMS4wNSAxLjctLjE2IDMuMjUuMjNzMi42Mi42MyA0LjQ5IDEuNzJjMS44NyAxLjA4IDIuODkgMS45MSA0Ljg0IDMuNjkgMS45NSAxLjc3IDIuNzcgMy4yIDQuOTEgNS4xOCAyLjEzIDEuOTggMy40OSAzLjM3IDUuNzYgNC43MyAyLjI2IDEuMzYgMy4yMyAxLjY3IDUuNTQgMi4wNyAyLjMxLjQgMy40OS4zMiA2LS4wNyAyLjUtLjM5IDQtLjg2IDYuNTMtMS44NyAyLjUzLTEuMDIgMy43LTIuMDMgNi4xMi0zLjIgMi40Mi0xLjE4IDMuNjMtMS45NSA1Ljk5LTIuNjcgMi4zNS0uNzIgMy40Ni0uOTggNS43OC0uOTQgMi4zMi4wNSAzLjM5LjM2IDUuODMgMS4xOHMzLjc2IDEuNDEgNi4zNyAyLjk0YzIuNjEgMS41NCAzLjkgMi41MSA2LjY4IDQuNzQgMi43OCAyLjIzIDQuNDcgMy45NyA3LjIxIDYuNDEgMi43NCAyLjQzIDQuMjQgNC4wMSA2LjQ5IDUuNzcgMi4yNCAxLjc2IDMuNTUgMi42NCA0LjcyIDMuMDEgMS4xOC4zOCAxLjU0LjA1IDEuMTUtMS4xNS0uMzktMS4xOS0xLjE4LTIuNjgtMy4xMS00LjgyLTEuOTItMi4xNC0zLjczLTMuNDItNi41Mi01Ljg5LTIuNzktMi40Ny00LjU0LTQuMTEtNy40My02LjQ1LTIuODgtMi4zMy00LjE3LTMuNDYtNi45OS01LjIzLTIuODItMS43OC00LjI0LTIuNjYtNy4xLTMuNjQtMi44NS0uOTktNC4zMS0xLjE5LTcuMTgtMS4yOS0yLjg2LS4xLTQuMzQuMTItNy4xNC44MS0yLjgxLjY4LTQuMzIgMS40NS02Ljg5IDIuNjEtMi41OCAxLjE1LTMuNzIgMi4wOC02IDMuMTUtMi4yOSAxLjA3LTMuNDcgMS42NC01LjQ0IDIuMjEtMS45Ny41OC0yLjgxLjkzLTQuNDIuNjUtMS42Mi0uMjctMS45OC0uNjctMy42NS0yLjAyLTEuNjYtMS4zNS0yLjc0LTIuNzEtNC42Ni00LjczLTEuOTMtMi4wMi0yLjgzLTMuMzktNC45Ny01LjM4LTIuMTQtMS45OS0zLjMxLTMuMjMtNS43My00LjU3LTIuNDEtMS4zMy00LjA1LTEuODgtNi4zMy0yLjEyLTIuMjctLjI0LTMuNTguMjgtNS4wNC45Mi0xLjQ2LjY1LTEuOTggMS40OS0yLjI1IDIuMy0uMjcuODEuMjQgMS4zOS44OCAxLjczTTg0MS4yIDUwMi45OWMtLjM5Ljg5LS42OCAxLjUyLS4zNSA0LjE0LjMyIDIuNjMgMS4wNiA0LjMxIDEuOTYgOC45OS45IDQuNjggMS41NCA3Ljk4IDIuNTIgMTQuMzkuOTcgNi40MSAxLjQ3IDEwLjQ3IDIuMzUgMTcuNjcuODggNy4yMSAxLjI0IDExLjQ4IDIuMDUgMTguMzUuODEgNi44NyAxLjIyIDEwLjI1IDIuMDIgMTYuMDEuOCA1Ljc1IDEuMDUgOC4zNyAxLjk4IDEyLjc2LjkzIDQuNCAxLjExIDYuNCAyLjY4IDkuMjEgMS41OCAyLjggMi42MyAzLjkxIDUuMTkgNC44IDIuNTYuODkgNC4xNyAxLjAzIDcuNjMtLjM3IDMuNDYtMS4zOSA1LjAzLTMuMTQgOS42OC02LjYxIDQuNjQtMy40OCA3LjQxLTYuMDUgMTMuNTUtMTAuNzUgNi4xNS00LjcxIDEwLjE5LTcuNDQgMTcuMTYtMTIuNzcgNi45Ny01LjMyIDEwLjk2LTguNjkgMTcuNjktMTMuODcgNi43My01LjE3IDEwLjUzLTcuNzMgMTUuOTYtMTIuMDIgNS40My00LjI4IDcuOTMtNi4yMyAxMS4yLTkuNDIgMy4yNi0zLjE4IDQuMy01LjAzIDUuMTItNi41MS44Mi0xLjQ3LjI4LTEuODgtMS4wMy0uODctMS4zIDEuMDEtMi4xOSAyLjg2LTUuNDkgNS45Mi0zLjI5IDMuMDYtNS42MiA1LjA5LTEwLjk4IDkuNC01LjM3IDQuMy05LjEyIDYuOTUtMTUuODMgMTIuMTQtNi43MSA1LjE5LTEwLjcxIDguNTUtMTcuNzEgMTMuODEtNy4wMSA1LjI3LTExLjEgNy45Ni0xNy4zMyAxMi41Mi02LjI0IDQuNTYtOS4yIDcuMDgtMTMuODUgMTAuMjgtNC42NSAzLjItNi40MyA0LjQ2LTkuNCA1LjczLTIuOTYgMS4yOC0zLjY4IDEuMjMtNS40Mi42My0xLjc0LS41OS0yLjAzLTEuMjMtMy4yOS0zLjYtMS4yNS0yLjM3LTEuOS00LjEtMi45Ny04LjI1LTEuMDYtNC4xNC0xLjQ1LTYuOC0yLjM2LTEyLjQ5LS45LTUuNjgtMS4zMy05LjA3LTIuMTUtMTUuOTItLjgyLTYuODYtMS4xNy0xMS4xMy0xLjk1LTE4LjM1LS43OS03LjIzLTEuMjEtMTEuMy0xLjk2LTE3Ljc3LS43NS02LjQ3LTEuMTYtOS44My0xLjgtMTQuNTgtLjYzLTQuNzUtLjc0LTYuNTktMS4zOS05LjE3LS42NS0yLjU4LTEuMTctMy4wNS0xLjg3LTMuNzQtLjY5LS42OC0xLjIxLS41OC0xLjYxLjMxIiBzdHJva2U9IiMwMDAiLz48cGF0aCBkPSJNOTExLjU0IDU1NS41NWMtLjI2IDEuMTEtLjU3IDIuNS40NCA1LjAxIDEuMDEgMi41MiAyLjEyIDQuMiA0LjYxIDcuNTggMi40OCAzLjM4IDQuMTkgNS42MyA3LjgxIDkuMzIgMy42MyAzLjY5IDUuOTIgNS45NCAxMC4zIDkuMTQgNC4zOCAzLjIgNi45MyA0LjggMTEuNiA2Ljg2IDQuNjYgMi4wNiA3IDIuNjUgMTEuNzIgMy40MyA0LjcyLjc5IDcuMjQuODYgMTEuODkuNTIgNC42Ni0uMzUgNy4wNi0uODEgMTEuMzctMi4yNiA0LjMtMS40NCA2LjMyLTIuNjYgMTAuMTctNC45NiAzLjg0LTIuMzEgNS43Ni0zLjkyIDkuMDYtNi41NyAzLjI5LTIuNjQgNC45Mi00LjI5IDcuNDEtNi42NSAyLjQ5LTIuMzYgMy40LTMuNzkgNS4wMi01LjEzIDEuNjEtMS4zMyAxLjgtMS44OCAzLjA3LTEuNTYgMS4yNy4zMyAxLjczIDEuNDcgMy4yNiAzLjE5IDEuNTMgMS43MiAyLjYzIDMuNTcgNC40IDUuNDEgMS43NiAxLjgzIDIuODIgMi42NiA0LjQyIDMuNzYgMS42MSAxLjExIDIuNjggMS42NCAzLjYyIDEuNzcuOTMuMTIgMS4yMi0uMjQgMS4wOC0xLjE0LS4xNC0uOS0uOC0xLjczLTEuNzgtMy4zNy0uOTgtMS42NC0xLjQtMi44Mi0zLjExLTQuODQtMS43Mi0yLjAyLTMuMTgtMy43MS01LjQ3LTUuMjctMi4yOS0xLjU3LTMuNjctMi4zNy01Ljk5LTIuNTUtMi4zMi0uMTgtMy4zOC4yNS01LjYxIDEuNjYtMi4yMiAxLjQtMy4wMyAyLjkzLTUuNTIgNS4zNy0yLjQ4IDIuNDUtMy44IDQuMTgtNi44OSA2Ljg1cy00LjkzIDQuMjQtOC41NCA2LjVjLTMuNjIgMi4yNS01LjUgMy4zOC05LjU0IDQuNzktNC4wNCAxLjQtNi4yNyAxLjg0LTEwLjY1IDIuMjEtNC4zNy4zNy02Ljc3LjM1LTExLjI0LS4zNy00LjQ2LS43Mi02LjY2LTEuMjMtMTEuMDgtMy4yMS00LjQxLTEuOTgtNi44Ny0zLjUyLTExLTYuNjgtNC4xMy0zLjE1LTYuMzItNS40LTkuNjYtOS4wOC0zLjMzLTMuNjgtNC44MS02LjAyLTcuMDEtOS4zMy0yLjItMy4zLTIuNzEtNS4wMS0zLjk5LTcuMi0xLjI5LTIuMi0xLjYtMy4xMy0yLjQzLTMuNzctLjg0LS42NC0xLjQ4LS41NS0xLjc0LjU3TTk5NS45NyA1MTUuNjJjLjQyLS40MS0uMDMtLjQ1LS4yLS40OC0uMTctLjAzLS4zMS40OC0uNjUuMzMtLjMzLS4xNS0uNTEtMS4xMS0xLjA0LTEuMDctLjUzLjA0LTEuNTQuNy0xLjYyIDEuMjctLjA3LjU3LjU1IDEuNTcgMS4yNSAxLjU2LjctLjAxIDEuODUtMS4xOSAyLjI2LTEuNjFNMTA0Ny42OSA1NjYuMzVjLjIxIDEuMi43NyAyLjUxIDIuNDggNC43NiAxLjcyIDIuMjQgMy4zOSAzLjc4IDYuMDkgNi40NiAyLjcgMi42NyA0LjUgNC40MiA3LjQyIDYuOTEgMi45MSAyLjQ5IDQuMzcgMy44NyA3LjE4IDUuNTIgMi44MSAxLjY2IDQuMTUgMi4yNSA2Ljg3IDIuNzQgMi43My40OSA0LjAyLjMxIDYuNzUtLjMxIDIuNzMtLjYxIDQuMTgtMS4yOCA2LjktMi43OSAyLjcyLTEuNSAzLjg5LTIuODMgNi43MS00LjczIDIuODEtMS45IDQuMjctMy4xOCA3LjM3LTQuNzYgMy4xMS0xLjU5IDQuNzQtMi40MSA4LjE0LTMuMTcgMy40LS43NSA1LjE2LS44MiA4Ljg2LS42IDMuNzEuMjMgNS43My42NiA5LjY4IDEuNzMgMy45NSAxLjA4IDYgMS44OCAxMC4wNiAzLjY1IDQuMDcgMS43NiA2LjIgMy4yMSAxMC4yNyA1LjIgNC4wNyAxLjk4IDYuMDYgMy4yIDEwLjA4IDQuNzQgNC4wMiAxLjUzIDYuMjIgMi4xNyAxMC4wMSAyLjkyczUuODQuOTggOC45NC44NGMzLjExLS4xNCA0LjQ5LS4zNyA2LjU5LTEuNTMgMi4wOS0xLjE2IDMuMDItMi4zMyAzLjktNC4yOC44OS0xLjk0Ljk1LTMuMTkuNS01LjQ2LS40NC0yLjI2LTEuMDMtMy43MS0yLjcxLTUuODhzLTIuOTctMy40NC01LjY4LTQuOTdjLTIuNzItMS41Mi00Ljc2LTIuMDYtNy45LTIuNjUtMy4xMy0uNTgtNS4wOS0uNjMtNy43OS0uMjgtMi43MS4zNS00LjI3LjkyLTUuNzQgMi4wNC0xLjQ3IDEuMTItMS44OCAyLjItMS42MyAzLjU2LjI2IDEuMzUuODEgMi4xNyAyLjkyIDMuMjIgMi4xMiAxLjA2IDMuNzEgMS4wMiA3LjY1IDIuMDYgMy45NCAxLjAzIDYuNzQgMS4zNyAxMi4wNiAzLjEzIDUuMzMgMS43NyA4LjYzIDIuNzkgMTQuNTggNS42OSA1Ljk0IDIuOSA5LjI0IDQuODcgMTUuMTUgOC44IDUuOTEgMy45MiA5LjIgNi4zNSAxNC4zOSAxMC44NCA1LjE5IDQuNSA3LjY5IDcuMDUgMTEuNTggMTEuNjIgMy45IDQuNTcgNS40OSA3LjA3IDcuODkgMTEuMjUgMi40IDQuMTggMy40NCA2LjIyIDQuMTEgOS42NC42OCAzLjQyLjM5IDQuODgtLjc0IDcuNDgtMS4xMiAyLjU5LTEuOTggMy43Mi00Ljg4IDUuNTEtMi45MSAxLjc5LTQuNzQgMi41Mi05LjY1IDMuNDMtNC45LjkxLTguMjUgMS4xNi0xNC44NiAxLjE0LTYuNjItLjAxLTEwLjUtLjMxLTE4LjIyLTEuMjMtNy43My0uOTEtMTIuMjgtMS43LTIwLjQyLTMuMzUtOC4xNC0xLjY2LTEyLjQ4LTIuOC0yMC4yOS00LjktNy44Mi0yLjEtMTEuOTQtMy40My0xOC43OS01LjU5LTYuODUtMi4xNy0xMC4xMy0zLjE2LTE1LjQ3LTUuMjUtNS4zMy0yLjA5LTcuOC0zLjIzLTExLjE5LTUuMjMtMy4zOC0xLjk5LTQuODItMy4wOS01LjcyLTQuNzYtLjg5LTEuNjcuMDEtMi4xNiAxLjI1LTMuNiAxLjI0LTEuNDMgMi45My0yLjI4IDQuOTYtMy41OCAyLjAzLTEuMjkgMy4yNi0xLjggNS4xOS0yLjg5IDEuOTQtMS4xIDMuNjktMS42OCA0LjQ4LTIuNTguNzgtLjkuNzEtMS41OS0uNTQtMS45My0xLjI1LS4zNC0zLjMxLS40NS01LjcuMjUtMi4zOS42OS0zLjk5IDEuNDMtNi4yNSAzLjIyLTIuMjYgMS43OC0zLjg5IDMuMjMtNS4wNiA1LjcxLTEuMTggMi40Ny0yLjAyIDQuMTctLjgxIDYuNjZzMy4xNCAzLjY1IDYuODcgNS44YzMuNzMgMi4xNCA2LjI5IDIuOTMgMTEuNzggNC45MSA1LjQ5IDEuOTggOC43NiAyLjkgMTUuNjcgNS4wMSA2LjkxIDIuMSAxMS4wMyAzLjQxIDE4Ljg5IDUuNSA3Ljg1IDIuMDkgMTIuMiAzLjI0IDIwLjM4IDQuOTQgOC4xOCAxLjcgMTIuNzQgMi41NCAyMC41MyAzLjU2IDcuNzkgMS4wMyAxMS42NyAxLjQxIDE4LjQzIDEuNTcgNi43NS4xNyAxMC4xMi4xMSAxNS4zNS0uNzIgNS4yMy0uODQgNy40LTEuMzkgMTAuNzktMy40NyAzLjQtMi4wNyA0LjgyLTMuNjcgNi4xOC02LjkgMS4zNS0zLjI0IDEuNDUtNS4zNy42MS05LjI4LS44My0zLjkyLTIuMTYtNS45Ni00LjgtMTAuMy0yLjYzLTQuMzUtNC4zMS02Ljc4LTguMzYtMTEuNDEtNC4wNC00LjYzLTYuNTktNy4xOS0xMS44OC0xMS43NC01LjI5LTQuNTYtOC42LTYuOTktMTQuNTYtMTEuMDMtNS45Ny00LjAzLTkuMjktNi4wNC0xNS4yNi05LjE0LTUuOTgtMy4xLTkuMzEtNC4yNC0xNC42Mi02LjM1LTUuMzEtMi4xMi04LjA2LTIuOTQtMTEuOTMtNC4yMi0zLjg2LTEuMjctNS4zNC0xLjc1LTcuMzgtMi4xNy0yLjA0LS40Mi0yLjU0LjAyLTIuODIuMDYtLjI4LjA1LjE3LjE2IDEuNDEuMTcgMS4yNC4wMiAyLjUzLS4xNCA0Ljc5LS4xMSAyLjI2LjAzIDMuOTUtLjIzIDYuNTIuMjcgMi41Ni41IDQuMTYgMS4wOCA2LjMyIDIuMjMgMi4xNSAxLjE1IDMuMDYgMi4wNiA0LjQ1IDMuNTMgMS4zOSAxLjQ3IDEuOTMgMi40NSAyLjUgMy44My41OCAxLjM3Ljc4IDEuOTUuMzkgMy4wNC0uNCAxLjEtLjg2IDEuODEtMi4zNyAyLjQxLTEuNTEuNjEtMi41Mi41My01LjE5LjYyLTIuNjguMDgtNC42NS4zNC04LjE5LS4xOS0zLjU0LS41My01LjY0LTEuMDUtOS41MS0yLjQ1LTMuODctMS40LTUuOC0yLjU3LTkuODQtNC41My00LjA0LTEuOTctNi4yLTMuNDYtMTAuMzYtNS4zLTQuMTYtMS44My02LjMtMi43MS0xMC40NS0zLjg5LTQuMTUtMS4xOC02LjI4LTEuNy0xMC4zLTIuMDEtNC4wMy0uMzEtNi4wNC0uMjgtOS44My40Ni0zLjc4LjczLTUuNjggMS42Mi05LjEgMy4yLTMuNDEgMS41OC01LjA1IDIuOS03Ljk3IDQuNzFzLTQuMTUgMi45Mi02LjYzIDQuMzRjLTIuNDcgMS40Mi0zLjU4IDIuMS01LjczIDIuNzYtMi4xNi42Ni0yLjk0Ljk1LTUuMDMuNTYtMi4wOS0uNC0zLjAxLS45OS01LjQxLTIuNTQtMi40LTEuNTQtMy44Ni0yLjc4LTYuNTktNS4xOHMtNC40OC00LjE3LTcuMDYtNi44MWMtMi41OC0yLjY1LTMuOC00LjU1LTUuODQtNi40NC0yLjA1LTEuODgtMy4yMy0yLjY0LTQuMzktMi45OS0xLjE2LS4zNC0xLjY0LjA2LTEuNDMgMS4yNyIgc3Ryb2tlPSIjMDAwIi8+PC9zdmc+" height="auto" width="150">
  <br />
  </a>
     <a style="font-size:10px;color:#dedede;">owner</a> 
    </center> 	
	
	</el-link>
      </div>

    </div>
  </el-container>
  <el-dialog align-center style="width: 90%;max-width: 700px;" v-model="downLoadAPPTableVisible" title="APP下载">
    <div>
      <el-button style="float:right;margin-top: -5px;" type="primary" @click="open('https://api.netart.cn/d?b013x15cb')">
          下载最新版
      </el-button> 
      <h2>网络面板APP</h2>
      <span>Java原生实现</span><br> 
      <span>1.支持锁屏运行</span><br>
      <span>2.支持添加任何链接</span><br>
      <span>3.相对于浏览器更加省电</span><br>
      <span>4.通知栏实时查看网络信息</span><br>
    </div>
    <div>
      <h2>更新日志</h2>
	  <div>
        <h3>v3.2.1</h3>
        <p>
          1.添加链接时可选“增强并发”开关(v2.7~v3.1此功能全局开启)<br>
		  2.修复从通知栏退出后再打开总流量不清零问题<br>
		  3.修复部分链接暂停之后再启动没有速度的问题<br>
        </p>
      </div>
      <div>
        <h3>v3.1.0</h3>
        <p>
          修复了部分情况下卡第一屏的问题<br>
        </p>
      </div>
      <div>
        <h3>v3.0.1</h3>
        <p>
          1.通知栏新增开始暂停退出按钮<br>
          2.屏保模式新增电量显示<br>
          再次提示：App可以锁屏运行，不建议使用屏保模式（更耗电）
        </p>
      </div>
      <div>
        <h3>v2.7.1</h3>
        <p>
          1.多线程速度优化<br>
          2.全新的启动动画<br>
          3.缓存首页资源文件，启动更快<br>
        </p>
      </div>
      <div>
        <h3>v2.6</h3>
        <p>
          1.修复了线程数设置错误的问题<br>
          2.修复了运行一段时间后可能闪退的问题<br>
          3.修复了部分模拟器闪退的问题<br>
        </p>
      </div>
      <div>
        <h3>v2.5</h3>
        <p>
          1.省电优化<br>
          2.安装包体积优化<br>
        </p>
      </div>
      <div>
        <h3>v2.4</h3>
        <p>
          1.修复了大量的问题<br>
        </p>
      </div>
      <div>
        <h3>v2.3</h3>
        <p>
          1.新增上传测速功能<br>
            (建议不超过2个线程)<br>
        </p>
      </div>
      <div>
        <h3>v2.2</h3>
        <p>
          1.修复了启动闪白屏的问题<br>
          2.修复了打开后切换深色模式出现logo遮挡问题<br>
          3.修复了暂停可能不及时的问题<br>
          5.切换到okhttp请求库，提高性能与错误处理能力<br>
          6.通知样式调整<br>
          7.更省电<br>
        </p>
      </div>
      <div>
        <h3>v2.1</h3>
        <p>
        1.修复了2.0版本部分链接跑一会儿没速度的问题，修复了一个增加耗电的问题<br> 
        2.核心功能完全由原生Java层接管，省电不发热的同时可以保后台，实测小米6黑屏后台运行12小时不掉<br> 
        3.同步近期网页版更新内容<br> <br> 
        保后台条件:<br> 
        1.通知栏能够正常显示进度信息（如果没有看到通知，去设置检查通知权限）<br> 
        2.加入电池优化白名单（如果没有加入，打开app会弹窗要求加入）<br> 
        如果部分老旧机型打开白屏，请
        <el-link @click="open('https://api.netart.cn/d?b013x2a3i')" type="primary">点此下载</el-link>
        webview内核，并在开发者选项内启用该内核后重试
        </p>
      </div>
    </div>
  </el-dialog>
  <el-dialog style="width: 90%;max-width: 400px;" v-model="aboutVisible" title="关于">
    <div>
      <h2>网络面板</h2>
      <span>作者：<el-link @click='open("https://netart.cn/")' type="primary">Whoami</el-link></span><br>
      <span>QQ：<el-link type="primary" @click="copyText('582424565')">582424565 </el-link></span><br>
      <span>QQ群：<el-link type="primary" @click="copyText('463481772')">463481772 </el-link></span><br>
      <span>开源地址：<el-link @click='open("https://github.com/ljxi/NetworkPanel")' type="primary">NetworkPanel</el-link>&nbsp;
        <el-link @click='open("https://github.com/ljxi/GeoCN")' type="primary">GeoCN</el-link>
      </span><br> 
      <span>赞助支持：
        <el-link @click='open("https://afdian.net/a/ljxnet")' type="primary">爱发电</el-link>&nbsp
        <el-link @click='open("https://qr.alipay.com/fkx13781i79xywfarbvrsfc")' type="primary">支付宝</el-link>
      </span><br>
      <span>特别感谢：</span><br>
      <el-link @click='open("https://www.kuocaicdn.com/register?code=8z8urvbg2ffd9")' type="primary">括彩科技</el-link><span>提供免费稳定的CDN服务</span><br>
      <el-link @click='open("https://staticfile.org/")' type="primary">七牛云</el-link><span>提供免费稳定的前端静态资源分发服务</span><br>
      <el-link @click='open("https://www.bootcdn.cn/")' type="primary">BootCDN</el-link><span>提供免费稳定的前端静态资源分发服务</span><br>
      <br>
      <span>本项目用到的开源库:</span><br>
      <el-link @click='open("https://github.com/vuejs/core")' type="primary">Vue</el-link>&nbsp
      <el-link @click='open("https://github.com/element-plus/element-plus")' type="primary">ElementPlus</el-link>&nbsp
      <el-link @click='open("https://github.com/apache/echarts")' type="primary">echarts</el-link>&nbsp
      <el-link @click='open("https://github.com/richtr/NoSleep.js")' type="primary">NoSleep.js</el-link>&nbsp
      <el-link @click='open("https://github.com/soerenmartius/vue3-clipboard")' type="primary">vue3-clipboard</el-link>&nbsp
    </div>
    <div>
      <h2>疑问解答</h2>
      <div class="question">
        <span class="ask">问：APP/后端代码开源吗？</span><br>
        <span class="answer">答：不开源</span><br>
      </div>
      <div class="question">
        <span class="ask">问：我搭建了一个前端页面，能否添加到跨域白名单？</span><br>
        <span class="answer">答：你需要有一定的用户量，并添加链接指向本项目开源仓库，然后联系我加白名单</span><br>
      </div>
      <div class="question">
        <span class="ask">问：能否添加xxx功能？</span><br>
        <span class="answer">答：有合理的建议请联系我</span><br>
      </div>
    </div>
    <template #footer>
      <span class="dialog-footer">
        <el-button @click="aboutVisible = false">关闭</el-button>
      </span>
    </template>
  </el-dialog>
</template>

<script lang="ts" setup>
import MainUI from "./components/Main.vue"
import IPinfoUI from "./components/IPinfo.vue"
import { ref, reactive, watch } from 'vue'
import { ElMessage } from 'element-plus'
import { toClipboard } from '@soerenmartius/vue3-clipboard'
var isAndroid = /Android/i.test(navigator.userAgent)
const isVisible = ref(true)
const downLoadAPPTableVisible = ref(false)
if(window.location.hash=='#app')downLoadAPPTableVisible.value=true

const clearHash=()=>{
  history.replaceState(null, document.title,
  window.location.pathname + window.location.search);
}
watch(downLoadAPPTableVisible,(n)=>{
  if(!n){
    clearHash()
  }else{
    window.location.hash='#app'
  }
})

const aboutVisible = ref(false)
const open = (url:string) => {
  window.open(url)
}

let copyText = (txt:string) => {
  toClipboard(txt)
  ElMessage.info({
    dangerouslyUseHTMLString: true,
    message: '<center>已经复制到剪切板</center>',
  })
}
document.addEventListener("visibilitychange", function () {
  var string = document.visibilityState
  if (string === 'hidden') isVisible.value = false
  else isVisible.value = true
})
</script>

<style scoped>  
.question {
  margin-top: 10px;
}
.ask {
  color: #6071ee;
}
.header {
  height: fit-content;
  padding-bottom: 12px;
  background-color: #ffffff;
}

.title {
  color: #526484;
  font-size: 20px;
  font-weight: bolder;
}

.home {
  color: #526484;
  font-size: 12px;
}
.icon {
  display:inline-block;
  vertical-align: -6px;
  width: 40px;
  height: 40px;
  background-color: #5668EE;
  border-radius: 20%;
}
.icon svg {
  width: 30px;
  margin-left: 5px;
}
.card{
    max-width: 800px;
    height:fit-content;
    display: block;
    margin:0 auto;
    background-color:#ffffff;
    padding:2%;
    border-radius: 20px;
}
.banner{
  margin-top: 15px;
}
.banner > img {
  height: 70px;
  width: calc(100% - 20px);
  margin: 10px;
  border-radius: 20px;
}
.banner > span{
  position: relative;
  display: block;
  left: 15px;
  top: 10px;
  color: transparent;
  font-weight: bolder;
  background-clip: text;
  background-image: linear-gradient(to right,#37CAC6, #3D95F4 80px);

}
@media (prefers-color-scheme: dark) {
  .card {
        background-color:rgb(18,18,18);
    }
  .header {
    background-color: rgb(18, 18, 18);
  }

  .title {
    color: rgb(152, 167, 202);
  }

  .home {
    color: rgb(152, 167, 202);
  }
}</style>
