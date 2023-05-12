bla = process.cwd()

var fs = require('fs')
var hx = require('hxz-api');
var axios = require('axios')
var multer = require('multer')
var Ddos = require('ddos')
var express = require('express')
var request = require('request');
var cheerio = require('cheerio');
var { fromBuffer } = require('file-type')
var exec = require('child_process').exec;
cors = require('cors')

const PORT = process.env.PORT || 3000

var ddos = new Ddos({burst:4, limit:30, testmode:true, whitelist:['187.21.11.237']});

// Def. onde fica os [ Token de Consultas ]
var tokenc = ["@TeddyDomina"]


//-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-\\

const router = express.Router();

var upload = multer()

var app = express()
 
app.use(cors())
app.set("json spaces",2)
app.use(express.static("public"))

var blacklist = require('express-blacklist');
app.use(blacklist.blockRequests('blacklist.txt'));

////PAGINA INICIAL Q IRA REDIRECIONAR PRA /DOC
 
router.use(ddos.express);
app.get("/", (req,res,next) => {
console.log("Beep");
res.end("Boop");
})
app.use(router);

 
//  CONSULTAS  \\

  app.get('/puxar/nome', async(req, res, next) => {    
token = req.query.token
nome = req.query.nome
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
if (!nome) return res.json({ status : false, msg : "Está faltando o parametro nome."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/nome?token=@TeddyModz&nome=${nome}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

 app.get('/puxar/nome2', async(req, res, next) => {    
token = req.query.token
nome = req.query.nome
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
if (!nome) return res.json({ status : false, msg : "Está faltando o parametro nome."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/nome2?token=@TeddyModz&nome=${nome}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf2', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf2?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf3', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf3?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf4', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf4?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf5', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf5?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

var resultado = hasil.result;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf6', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf6?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

var resultado = hasil.result;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cpf7', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf7?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

var resultado = hasil.result;
             res.json({
                 status: true,
                 
                 token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

  app.get('/puxar/cpf8', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cpf8?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

var resultado = hasil.result;
             res.json({
                 status: true,
                 
                 token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/score', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/score?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

  app.get('/puxar/vizinhos', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/vizinhos?token=@TeddyModz&cpf==${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

  app.get('/puxar/parentes', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/parentes?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

  app.get('/puxar/benefícios', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
 if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/beneficios?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
                 
token: `${token}`,
                 resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/tel', async(req, res, next) => {    
token = req.query.token
telefone = req.query.telefone
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!telefone) return res.json({ status : false, msg: "Está faltando o parametro telefone."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/tel?token=@TeddyModz&telefone=${telefone}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/tel2', async(req, res, next) => {    
token = req.query.token
telefone = req.query.telefone
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!telefone) return res.json({ status : false, msg: "Está faltando o parametro telefone."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/tel2?token=@TeddyModz&telefone=${telefone}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/tel3', async(req, res, next) => {    
token = req.query.token
telefone = req.query.telefone
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!telefone) return res.json({ status : false, msg: "Está faltando o parametro telefone."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/tel3?token=@TeddyModz&telefone=${telefone}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cnpj', async(req, res, next) => {    
token = req.query.token
cnpj = req.query.cnpj
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!cnpj) return res.json({ status : false, msg: "Está faltando o parametro cnpj."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cnpj?token=@TeddyModz&cnpj=${cnpj}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

app.get('/puxar/cnpj2', async(req, res, next) => {    
token = req.query.token
cnpj = req.query.cnpj
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!cnpj) return res.json({ status : false, msg: "Está faltando o parametro cnpj."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cnpj2?token=@TeddyModz&cnpj=${cnpj}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/placa', async(req, res, next) => {    
token = req.query.token
placa = req.query.placa
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!placa) return res.json({ status : false, msg : "Está faltando o parametro placa."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/placa?token=@TeddyModz&placa=${placa}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

   app.get('/puxar/placa2', async(req, res, next) => {    
token = req.query.token
placa = req.query.placa
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!placa) return res.json({ status : false, msg : "Está faltando o parametro placa."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/placa?token=@TeddyModz&placa=${placa}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/vizinhos', async(req, res, next) => {    
token = req.query.token
cpf = req.query.cpf
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if (!cpf) return res.json({ status : false, msg: "Está faltando o parametro cpf."}) 
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/vizinhos?token=@TeddyModz&cpf=${cpf}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/bin', async(req, res, next) => {    
token = req.query.token
bin = req.query.bin
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if(!bin)return res.json({status:false, motivo:'Está faltando o parâmetro bin.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/bin?token=@TeddyModz&bin=${bin}`))
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/cep', async(req, res, next) => {    
token = req.query.token
code = req.query.code
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if(!code)return res.json({status:false, motivo:'Está faltando o parâmetro cep.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cep?token=@TeddyModz&code=${code}`))
    .then(response => response.json())
        .then(hasil => {
        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/puxar/banco', async(req, res, next) => {    
token = req.query.token
code = req.query.code
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if(!code)return res.json({status:false, motivo:'Está faltando o parâmetro code.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/banco?token=@TeddyModz&code=${code}`))        
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

    app.get('/api/geradores/banco', async(req, res, next) => {    
token = req.query.token
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/banco?token=@TeddyModz&code=${code}`))        
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.result;
             res.json({
                 status: true,
              token: `${token}`,
                                                     resultado
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

   app.get('/puxar/ip', async(req, res, next) => {    
token = req.query.token
code = req.query.code
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if(!code)return res.json({status:false, motivo:'Está faltando o parâmetro code.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/ip?token=@TeddyModz&code=${code}`))        
    .then(response => response.json())
        .then(hasil => {

        var info = hasil.info;
        var infoCidade = hasil.infoCidade
        var infoWifi = hasil.infoWifi
             res.json({
                 status: true,
              token: `${token}`,
                                                     info,
                   infoCidade,
                   infoWifi
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

   app.get('/puxar/ibge', async(req, res, next) => {    
token = req.query.token
code = req.query.code
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o !  wa.me/558171185449`})
if(!code)return res.json({status:false, motivo:'Está faltando o parâmetro code.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/ibge?token=@TeddyModz&code=${code}`))        
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
        var regiao = hasil.regiao
             res.json({
                 status: true,
              token: `${token}`,
resultado,
                   regiao
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

   app.get('/puxar/cns', async(req, res, next) => {    
token = req.query.token
code = req.query.code
if(!token)return res.json({status:false,msg:'Está faltando o parametro token.'})
  if(!tokenc.includes(token))return res.json({status: 404, mensagem: `O token "${token}" não foi encontrado! Compre um com o Teddy!  wa.me/558171185449`})
if(!code)return res.json({status:false, motivo:'Está faltando o parâmetro code.'})
  if(tokenc.includes(token)){
    fetch(encodeURI(`https://japa-puxadas.herokuapp.com/puxar/cns?token=@TeddyModz&cns=${code}`))        
    .then(response => response.json())
        .then(hasil => {

        var resultado = hasil.resultado;
        var regiao = hasil.regiao
             res.json({
                 status: true,
              token: `${token}`,
resultado,
                   regiao
             })
         })
         .catch(e => {
         	res.json({erro:'Erro no Servidor Interno'})
})
} else {
  res.json({erro:'Erro no Servidor Interno'})
}
})

////FUNÇAO DE PAGINA Q NAO TEM FUNÇÃO SOBRE ELA
app.get('*', function(req, res) {
res.status(404).json({
status: false,
aviso: 'PÁGINA NÃO ENCONTRADA!',
apisMe: ''
})
})
 
//////MOSTRA SE O APP FOI ABERTO
app.listen(PORT, () => {
console.log('Aplicativo aberto na porta: ' + PORT)
})


module.exports = router;