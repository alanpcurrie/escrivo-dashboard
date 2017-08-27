<template>
    <div id="card">
        <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Heigo</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--no-status">No status</button>
            </div>
        </div>

            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                <p class = "m-card--author__text">Alasdair</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--no-status">No status</button>
            </div>
        </div>

            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Cameron</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--no-status">No status</button>
            </div>
        </div>
            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Cameron</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--no-status">No status</button>
            </div>
        </div>
            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Aileen</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--no-status">No status</button>
            </div>
        </div>
            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Cameron</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--needs-work">Needs work</button>
            </div>
        </div>
            <div class="m-card__row">
            <div class="m-card">
                <h3 class="m-card__title">
                    making time for personal development
                </h3>
                <h3 class="m-card__text">
                    To ensure we find ways to continually improve ourselves and our capability, we need to make time for personal development and training.
                </h3>
            </div>
            <div class="m-card--author">
                 <p class = "m-card--author__text">Cameron</p>
            </div>
            <div class="m-card--status">
                <button class="a-btn--on-target">On target</button>
            </div>
        </div>
    </div>

    
</template>

<script>
export default {
    name: 'card',

}

</script>




<style>

@define-mixin red {
    /* background-color:red;  @add-mixin red; */
}

 &--new {
    @add-mixin red;
    }

.m-card__row {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr;
    grid-column-gap: 0.5rem;
    grid-row-gap: 0.5rem;
    margin-top: 1rem;
    margin-bottom: 1rem;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    transition: all 0.3s cubic-bezier(.25, .8, .25, 1);

}

@media screen and (max-width: 800px) {
   .m-card__row {
    display: grid;
    grid-template-columns: 100%;
    margin-top: 0.2rem;
    margin-bottom: 0.2rem;
    }
}

.m-card__row:hover {
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.10), 0 5px 5px rgba(0, 0, 0, 0.20);
}

.m-card {
    grid-column: 1 / span 1;
    padding: 1rem;
}

.m-card--author {
    margin-top: 2.2rem; 
    padding: .5rem;
}

.m-card--author__text {
     text-align: center;
     font-size: calc(80% + 0.5vw);    

}

.m-card--author__text:before {

    content: " ";
    background: url( '../assets/assignee.svg') no-repeat;
    background-position: center center;
    background-size: contain;
    padding: 0.45rem;
    margin-right: 0.2rem;

}

.m-card--status {
    text-align: center;
    padding: 1rem;
}

.m-card__title {
    font-size: calc(95% + 0.5vw);   
    font-weight: bold;
}

.m-card__text {
    font-size: calc(55% + 0.5vw);  
	line-height: 1.5;
    font-weight: lighter;
    color: darkslategrey;
    max-width: 700px;
}



.a-btn--no-status {
     min-width: 150px;
    white-space:nowrap;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: var(--color-white);
    border: 8px solid var(--color-grey);
    font-size: calc(70% + 0.5vw); 
    font-weight: bold;
    font-family: Montserrat, sans-serif;
    transition: all 0.3s cubic-bezier(.25, .8, .25, 1);

}

.a-btn--no-status:hover {
   
}

.a-btn--needs-work {
    min-width: 150px;;
    white-space:nowrap;
    flex-direction: column;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: var(--color-white);
    border: 8px solid var(--color-orange);
    font-size: calc(70% + 0.5vw);  
    font-weight: bold;
    font-family: Montserrat, sans-serif;
   
}

.a-btn--on-target {
    min-width: 150px;;
    white-space:nowrap;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: var(--color-white);
    border: 8px solid var(--color-green);
    font-size: calc(70% + 0.5vw); 
    font-weight: bold;
    font-family: Montserrat, sans-serif;
}
</style>
