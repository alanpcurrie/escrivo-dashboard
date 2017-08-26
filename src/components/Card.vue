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
                <p>Heigo</p>
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
                <p>Alasdair</p>
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
                <p>Cameron</p>
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
                <p>Cameron</p>
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
                <p>Aileen</p>
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
                <p>Cameron</p>
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
                <p>Cameron</p>
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

<style lang="postcss" scoped>
.m-card__row {
    display: grid;
    grid-template-columns: 70% 15% 15%;
    margin-top: 1rem;
    margin-bottom: 1rem;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    transition: all 0.3s cubic-bezier(.25, .8, .25, 1);
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
    text-align: center;
    padding: 1rem;
}

.m-card--status {
    text-align: center;
    padding: 1rem;
}

.m-card__title {
    font-size: 1.5rem;
    font-weight: bold;
}

.m-card__text {
    font-size: 1rem;
    font-weight: lighter;
    color: darkslategrey;
    max-width: 700px;
}

.a-btn--no-status {
     max-width: 1fr;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: white;
    border: 8px solid lightgray;
    font-size: 1rem;
    font-weight: bold;
    font-family: Montserrat, sans-serif;
}

.a-btn--needs-work {
    max-width: 1fr;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: white;
    border: 8px solid #EA7E3D;
    font-size: 1rem;
    font-weight: bold;
    font-family: Montserrat, sans-serif;

}

.a-btn--on-target {
     max-width: 1fr;
    margin-top: 2.2rem;
    padding: 0.2rem 1rem 0.2rem 1rem;
    background-color: white;
    border: 8px solid #1BAF54;
    font-size: 1rem;
    font-weight: bold;
    font-family: Montserrat, sans-serif;
}
</style>
