<script>
    import { each } from "svelte/internal";

    let allSrc = [
        "Wallpapers/TrueMan_Ancient_India_8k_hyper_realistic_cinematic_detailed_3f8c1b8a-adac-4360-b64a-9a2f78149a1c.png",
        "Wallpapers/sophisticated_italian_design_for_surface_pattern_with_m_b2be5ba9-b534-40e3-ac90-c037291bc432.png",
        "Wallpapers/sophisticated_italian_design_surface_pattern__0cc57808-d487-4a02-8bf6-954c609e43ab.png",
        "Wallpapers/TrueMan_cherry_blossoms_overlooking_the_sun_ancient_japan_vecto_1d6a1764-d025-44a3-8c60-5385f67024b7.png",
        "Wallpapers/PaperMan_enviromen_victorian_old_cottage_high_tree_besides_anti_e253b994-e236-497d-9fc9-4b38c027d8b2.png",
        "Wallpapers/PaperMan_Teacup_filled_with_tea_in_a_table_overlooking_an_open__631c7c1e-8db4-4f5a-b37c-ef38be22bd50.png",
        "Wallpapers/Lolic25_Arrakis_during_Sunset_DUNE_Ghibli_Miyazaki_640bd1e3-429d-4c62-888e-3cc467ef86b0.png",
        "Wallpapers/PaperMan_Dune_Paul_Atriedes_alone_in_the_desert_Timothe_Chalame_db7d5f1f-00e1-4c70-8b84-059ab1262d23.png",
        "Wallpapers/Chainsaw_Most_beautiful_woman_charlie_bowater_style__black_peta_40a5afa3-59a9-44ea-845a-cc5231c35f9f.png",
        "Wallpapers/Chainsaw_Most_beautiful_woman_charlie_bowater_style__black_peta_b3a0d13d-ee22-4f01-9930-86930c3a74b5.png",
        "Wallpapers/Chainsaw_Most_beautiful_woman_Close_up_profile_A_flowerpunk_Cyb_4166bb5c-6ad0-4538-b184-5da027930719.png",
        "Wallpapers/ChickenMan_Zelda_airy_pin-up_sci-fi_steam_punk_very_deitaled_re_28adaa1a-d665-4b3a-9488-07c5dbe1125c.png",
        "Wallpapers/ChickenMan_tarot_card_art_Art_Nouveau_style_b36ab913-6739-40d5-864c-59299570b0cf.png",
        "Wallpapers/ChickenMan_The_Fremen_Mesiah_Arrakis_DUNE_Minimalist_Grayscale__e3a7652e-363a-47a7-9562-58bc68189048.png",
        "Wallpapers/DilwaleDulhaniaLeJayenge_The_Hobbit_shire_Ultrarealistic_Detail_a80aa50f-d089-4a2f-b4f4-ab7f4155bcef.png",
        "Wallpapers/Muadib_Close-up_food_photography_of_hearty_Chicken_Tonkotsu_Ram_bacc1cfa-8634-4a12-88a4-36c354a63d79.png",
        "Wallpapers/Muadib_The_Fringe_in_the_style_of_the_artist_Laurie_Greasley_ru_7d9b7044-96a1-42b9-9b2a-99f8e97eccf3.png",
        "Wallpapers/Muadib_World_War_2_Plane_flying_alone_into_the_sunset_Ghibli_Cl_3607d803-a53b-46f6-a569-62e6848331ee.png",
        "Wallpapers/Supaa_Close-up_of_Siddhartha_Gautama_Buddhism_Goethe_9fbae395-3e90-431c-8c78-2e485b708241.png",
        "Wallpapers/Supaa_Wanderer_above_the_sea_of_fog_Caspar_David_Friedrich_6b73a74d-23dd-43f0-be42-85adb036e281.png",
        "Wallpapers/Supaa_Flowers_vector_art_minimalist_album_cover_d3151a40-6a6b-4fcc-8ed1-3cd1c1633c54.png",
    ];
</script>

<main>
    <div class="grid-container">
        {#each allSrc as ImgUrl}
        <div class="grid-item">
            <a href={ImgUrl} data-lightbox={ImgUrl}>
            <img src={ImgUrl} alt={ImgUrl} class="TrueImg">
            </a>
        </div>
        {/each}
    </div>
</main>

<style>
    .TrueImg{
        max-width: 100%;
    }
    .grid-container {
      margin-top: 5%;
      align-items: center;
      display: grid;
      grid-template-columns: 20% 20% 20% 20%;
      padding: 10px;
      gap: 5%;
    }
    .grid-item {
      background-color: rgba(255, 255, 255, 0.8);
      border-radius: 5%;
      overflow: hidden;
      font-size: 30px;
      text-align: center;
    }
    @media screen and (max-width: 600px){
        .TrueImg{
            max-width: 100%;
        }
        .grid-container {
            justify-content: center;
            align-items: center;
            display: grid;
            grid-template-columns: 55% 55%;
            padding: 10px;
            gap: 5%;
        }
    }
</style>
