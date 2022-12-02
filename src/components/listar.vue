<template>
    <div>
        <div v-for="s in students" :key="s.dni">
            <span>{{s.dni}}</span>
            <span>{{s.first}}</span>
            <span>{{s.family_name}}</span>
            <span>{{s.email}}</span>
            <span>{{s.age}}</span>
            <span>{{s.phone_number}}</span>
            <span>{{s.address}}</span>
        </div>
    </div>    

</template>
<script>
export default {
    data() {
        return {
            students: [
                {
                  dni:"",
                  first: "",
                  family_name: "",
                  email: "",
                  age:"",
                  phone_number:"",
                  address: "",


                },
                
            ]
        }
    },

    created:{

        
    },
mounted(){
    this.consultarStudents();
},
    methods: {

        consultarStudents() {
            fetch('http://localhost/Students/')
                .then(respuesta => respuesta.json())
                .then((datosRespuesta) => {
                    console.log(datosRespuesta)=>{

                        console.log(datosRespuesta)
                        this.Students = []
                        if (typeof datosRespuesta[0].success === 'undefined') {
                            this.Students = datosRespuesta;
                        }
                         }
                    })

                .catch(console.log)
        }


    }


}
</script>
