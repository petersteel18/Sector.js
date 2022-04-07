# Sector.js
Sector.js
var nome=window.prompt("Qual é o seu nome?")
 try{
 while(nome==null || nome.length==0){
 window.alert("[Erro] nome invalido, por favor digite o seu nome")
 nome=window.prompt("Qual é o seu nome?")
 }
 } catch(e){ while(nome==null || nome.length==0){
 window.alert("[Erro] nome invalido, por favor digite o seu nome")
 nome=window.prompt("Qual é o seu nome?")
 } 
 }
 window.alert(("Sejá bem vindo ")+ nome)
 window.alert("Esse programa foi desenvolvido por Diogo Alfredo Cabaça Umba")
 var n=[window.document.getElementById('txtn1'),window.document.getElementById('txtn2'),window.document.getElementById('txtn3'),window.document.getElementById('res'),,,,,window.document.getElementById('call')]//vector de 9 posições
 //chamada para a função calcular()
 function calcular(){
 if (n[0].value.length<=0 || n[1].value.length<=0 || n[2].value.length<=0){//Aplicando condições
 window.alert("[Erro] média invalida")//Começando com as mensagens de erro
 n[3].innerText='Impossível calcular'
 n[3].style.color='red'
 n[8].style.background='red'//Mudando a cor do site para vermelho
 n[8].style.color='#000'
 } else{//Caso as condiçôes acima forem falsa aplica-se esse bloco de instruções
 n[4]=Number(n[0].value)
 n[5]=Number(n[1].value)
 n[6]=Number(n[2].value)
 if (n[4]>n[5] && n[6]>n[5]){
 n[7]=(n[4]+n[6])/2
 }else if(n[4]>n[6] && n[5]>n[6]){
 n[7]=(n[4]+n[5])/2
 }else{
 n[7]=(n[5]+n[6])/2
 } n[3].innerText='A média dos dois maiores números é : '  +n[7]
  n[3].style.color='blue'
  n[8].style.background='rgb(70,142,236)'//Mudando a cor de fundo do site para a cor original
  n[8].style.color='white'//Mudando a cor de letra do site para branco
 }}
