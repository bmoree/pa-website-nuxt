<template>
  <main>
    <section class="hero">
      <div class="container">
        <div>
          <h1 class="text-4xl">
            Slimme oplossingen<br />
            voor complexe<br />
            processen
          </h1>

          <a href="/about">Lees meer</a>
        </div>
        <div>
          <img src="https://picsum.photos/200/300" alt="" />
        </div>
      </div>
    </section>
    <section class="container">
      <div
        class="
          -mt-48
          z-10
          py-16
          relative
          sm:grid sm:grid-cols-2
          lg:grid-cols-4
          grid-flow-row
          gap-8
        "
      >
        <div
          v-for="n in 4"
          :key="n"
          class="rounded-lg p-6 shadow-lg bg-white mt-4"
        >
          <h2>Some other title</h2>
          <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis
            corporis debitis iusto velit assumenda sint quia accusantium magnam
            quae fugit delectus, soluta iste earum illum! Nihil unde architecto
            quasi dolor libero voluptatem velit, temporibus ad consequuntur
            soluta aut fugiat possimus.
          </p>
        </div>
      </div>
    </section>
    <section class="py-12 container bg-gray-200">
      <h2>Some other title</h2>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis corporis
        debitis iusto velit assumenda sint quia accusantium magnam quae fugit
        delectus, soluta iste earum illum! Nihil unde architecto quasi dolor
        libero voluptatem velit, temporibus ad consequuntur soluta aut fugiat
        possimus.
      </p>
    </section>
  </main>
</template>
