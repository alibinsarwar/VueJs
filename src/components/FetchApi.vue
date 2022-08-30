<script setup>
window.addEventListener('DOMContentLoaded' , event => {

fetch('https://jsonplaceholder.typicode.com/todos')
.then(response => response.json())
.then(fetch => {
    fetch.forEach(fetch => {
        document.querySelector('#fetchApi').innerHTML += `<input type="checkbox" value="${fetch.id} id="${fetch.id}" ${ fetch.completed ? "checked" : ''} />
        <label for="${fetch.id}">${fetch.title}</label><br>`
    });
    getSelected()

    
    
})
.catch(err => console.log(err));
    

}
)
function getSelected(){
    selected = []

    checked = document.querySelectorAll('input[type="checkbox"]:checked')

    checked.forEach(chk => selected.push(chk.value))

    console.log(selected)
}

function CheckAll()
{

   var chk = document.querySelectorAll('input[type="checkbox"]')
    for (i = 0; i < chk.length; i++)
	chk[i].checked = true ;

}

function UnCheckAll()
{

   var chk = document.querySelectorAll('input[type="checkbox"]')
    for (i = 0; i < chk.length; i++)
	chk[i].checked = false ;

}


</script>
<template>
    <button>Save Updated List</button>
	<button id="chkAll" v-on:click="CheckAll">Check All</button>
	<button id="unChkAll" v-on:click="UnCheckAll">UnCheck All</button>
    <div id="fetchApi"></div>
</template>
