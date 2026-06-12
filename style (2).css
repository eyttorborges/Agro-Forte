// MENU MOBILE

const menuBtn = document.querySelector(".menu-mobile");
const navLinks = document.querySelector(".nav-links");

menuBtn.addEventListener("click", () => {
    navLinks.classList.toggle("active");
});

// CONTADORES

const counters = document.querySelectorAll(".counter");

const startCounter = () => {

    counters.forEach(counter => {

        const target = +counter.dataset.target;

        let count = 0;

        const increment = target / 150;

        const updateCounter = () => {

            if (count < target) {

                count += increment;

                counter.innerText =
                Math.floor(count).toLocaleString("pt-BR");

                requestAnimationFrame(updateCounter);

            } else {

                counter.innerText =
                target.toLocaleString("pt-BR");

            }
        };

        updateCounter();
    });
};

let contadorIniciado = false;

window.addEventListener("scroll", () => {

    const stats =
    document.querySelector(".estatisticas");

    const pos = stats.getBoundingClientRect().top;

    if(pos < window.innerHeight && !contadorIniciado){

        startCounter();

        contadorIniciado = true;
    }
});

// ANIMAÇÃO AO ROLAR

const reveals = document.querySelectorAll(".reveal");

function revealElements(){

    reveals.forEach(element => {

        const top = element.getBoundingClientRect().top;

        if(top < window.innerHeight - 100){

            element.classList.add("active");
        }
    });
}

window.addEventListener("scroll", revealElements);

revealElements();

// FORMULÁRIO

const form =
document.getElementById("formContato");

form.addEventListener("submit", function(e){

    e.preventDefault();

    const nome =
    document.getElementById("nome").value.trim();

    const email =
    document.getElementById("email").value.trim();

    const mensagem =
    document.getElementById("mensagem").value.trim();

    if(
        nome === "" ||
        email === "" ||
        mensagem === ""
    ){
        alert("Preencha todos os campos.");
        return;
    }

    if(!email.includes("@")){
        alert("Digite um e-mail válido.");
        return;
    }

    alert("Mensagem enviada com sucesso!");

    form.reset();

});