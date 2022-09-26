<template> 
  <header v-bind:class = "heading"> 
    <h2 v-bind:style = "{fontSize:size + 'px' , 
fontWeight:weis , paddingLeft:padd + 'px' , 
fontStyle:sty , textTransform:trans}">{{name}}</h2> 
    <div> 
        <ul v-bind:id = "mans"> 
            <li v-for = "nav in navs" :key = "nav"><a href = "#">{{nav}}</a></li>
        </ul>
    </div>
  </header> 
  <main v-bind:class = "boobs"> 
   <h3 v-bind:class = "damn">{{toggle ()}}</h3> 
   <button v-bind:class = "bush" v-on:click = "paras = 'the world of programmers'">Change Now</button>
   <h3 v-bind:style = "{marginTop:mag + 'px' , 
marginBottom:bog + 'px' , fontStyle:wos , 
fontWeight:beat}">{{followers}}</h3>
   <button v-bind:class = "dub" v-on:mouseover = "followers += 1">Count Now</button>
   
   <form v-bind:class = "gods" @submit = "submitForm"> 
    <input type="text" id = "username" placeholder="username" v-model = "formValues.username"> 
    <textarea v-bind:class = "pussy"  id="userinfo" placeholder="userinfo" v-model = "formValues.userinfo" cols="30" rows="10"></textarea>
    <select v-bind:class = "pop"  id="country" v-model = "formValues.country"> 
        <option value="">country</option> 
        <option value="arfghastian">Arfghastian</option> 
        <option value="america">America</option> 
        <option value="south america">South America</option> 
        <option value="south africa">South Africa</option> 
        <option value="tanzania">Tanzania</option>
    </select>   
    <select v-bind:class = "weed" id="jobLocation" v-model = "formValues.jobLocation"> 
      <option value="">jobLocation</option> 
      <option value="kenya">Kenya</option> 
      <option value="australia">Australia</option> 
      <option value="austria">Austria</option> 
      <option value="tanzania">Tanzania</option> 
    </select> 
    <input v-bind:class = "bug" type="checkbox"  id="remoteWork" v-model = "formValues.remoteWork" true-value = "yes" false-value = "no" >
      <label for="remoteWork">do you accept terms and conditions</label>
      <input v-bind:class = "mother" type="checkbox"  id="html" value = "html" v-model = "formValues.skillSet"> 
      <label for="html">HTML</label> 
      <input v-bind:class = "papa" type="checkbox"  id="css" value = "css" v-model = "formValues.skillSet"> 
      <label for="css">CSS</label> 
      <input v-bind:class = "momo" type="checkbox"  id="javascript" value = "javascript" v-model = "formValues.skillSet"> 
      <label for="javascript">JavaScript</label>
      <button v-bind:class = "papa" v-bind:id = "bad" onclick = "alert('you are hacked')" v-on:click = "name = 'Batman'">submit</button>
    </form>
  </main>
</template> 

<script> 
 export default{ 
    data(){ 
        return{ 
            name:'freelancers', 
            navs:['home' , 'about' , 'contact'], 
            size:18, 
            weis:800, 
            padd:10, 
            sty:'italic', 
            trans:'uppercase', 
            heading:'active', 
            mans:'navbar', 
            boobs:'butts', 
            paras:"The world of developers", 
            damn:'drama', 
            bush:'talk', 
            followers:0, 
            dub:'niggas',  
            mag:30, 
            bog:20, 
            wos:'italic', 
            beat:800, 
            gods:'search-box', 
            pussy:'good',  
            bad:'ass', 
            pop:'smoke', 
            weed:'bus', 
            bug:'broker', 
            mother:'better', 
            papa:'mak', 
            momo:'mama',
            formValues:{ 
                username:'',
                userinfo:'', 
                country:'', 
                jobLocation:[], 
                remoteWork:"no", 
                skillSet:[]
            }
        }
    }, 
    methods:{ 
        toggle(){ 
            return this.paras
        }, 
        submitForm(event){ 
           event.preventDefault() 
           console.log("form Values" , this.formValues)
        }
    }
 }
</script> 

<style lang = "css"> 
  *{ 
    margin:0; 
    padding:0; 
    box-sizing:border-box; 
    list-style:none; 
    text-decoration:none; 
    outline:none; 
    border:none; 
    font-family:'Poppin',sans-serif;
  } 
.active{ 
    width:100%; 
    padding:10px 15px; 
    display:flex; 
    align-items:center; 
    justify-content:space-between; 
    background:aquamarine; 
    box-shadow:2px 4px 4px rgba(200 , 10 , 0.5);
} 

#navbar{ 
      display:flex; 
      align-items:center; 
      justify-content:center; 
      flex-direction:column;
} 

#navbar li{ 
      margin:5px 0;
} 

#navbar li a{ 
      color:#000; 
      font-size:16px; 
      font-style:italic; 
      font-weight:800; 
      text-transform:capitalize; 
      transition:0.3s ease-in-out; 
      cursor:pointer; 
      font-style:italic;
} 

#navbar li a:hover{ 
    color:green;
} 

.butts{ 
     display:flex; 
     align-items:center; 
     justify-content:center; 
     flex-direction:column;
} 
.drama{ 
    font-size:16px; 
    letter-spacing:1.2px; 
    font-weight:800; 
    font-style:italic; 
    text-transform:uppercase; 
    margin:10px 0;
} 

.talk{ 
    width:100%;
    max-width:200px; 
    padding:10px 15px; 
    background:rgb(186, 11, 131); 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;  
    margin-top:10px;
    text-transform:uppercase; 
    cursor:pointer; 
    transition:0.3s ease-in-out; 
    border-radius:1rem; 
    box-shadow:2px 4px 4px rgba(200 , 10 , 0.5); 
} 

.talk:hover{ 
    color:#000; 
    background:#fff; 
    border:3px solid orange;
} 

.niggas{ 
    width:100%;
    max-width:200px; 
    padding:10px 15px; 
    background:rgb(48, 205, 77); 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;  
    margin-top:10px;
    text-transform:uppercase; 
    cursor:pointer; 
    transition:0.3s ease-in-out; 
    border-radius:1rem; 
    box-shadow:2px 4px 4px rgba(200 , 10 , 0.5); 
} 

.niggas:hover{ 
    color:#000; 
    background:#fff;
    border:3px solid orange;
} 

.search-box{ 
    display:flex; 
    align-items:center; 
    justify-content:center; 
    flex-direction:column;
} 

input{ 
    background:none; 
    appearance:none;
} 

input[type = "text"]{ 
    width:100%; 
    padding:10px 15px; 
    background:aquamarine; 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    border-radius:8px;
    margin-top:10px; 
    margin-bottom:10px;
}  

input[type = "text"]::placeholder{ 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;
}

.good{ 
    width:auto; 
    height:auto; 
    padding:10px; 
    border:2px solid #000; 
    border-radius:2px;
    font-size:18px; 
    font-weight:800; 
    font-style:italic;
}  

.good::placeholder{ 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    text-transform:capitalize;
}

#ass{ 
    width:100%;
    max-width:200px; 
    padding:10px 15px; 
    background:rgb(169, 26, 91); 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic;  
    margin-top:10px;
    text-transform:uppercase; 
    cursor:pointer; 
    transition:0.3s ease-in-out; 
    border-radius:1rem; 
    box-shadow:2px 4px 4px rgba(200 , 10 , 0.5);   
} 

#ass:hover{ 
    color:#000; 
    background:#fff; 
    border:3px solid orange;
} 

.smoke{ 
    width:100%; 
    padding:10px 15px; 
    background:aquamarine; 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    border-radius:8px;
    margin-top:10px; 
    margin-bottom:10px;
} 

.bus{ 
    width:100%; 
    padding:10px 15px; 
    background:rgb(47, 212, 110); 
    color:#000; 
    font-size:18px; 
    font-weight:800; 
    font-style:italic; 
    border-radius:8px;
    margin-top:10px; 
    margin-bottom:10px;
} 

.broker{ 
    width:auto; 
    height:auto; 
    border:1px solid #000; 
    border-radius:1px; 
    padding:5px;
} 

.better{ 
    width:auto; 
    height:auto; 
    border:1px solid #000; 
    border-radius:1px; 
    padding:5px;
} 

.mak{ 
    width:auto; 
    height:auto; 
    border:1px solid #000; 
    border-radius:1px; 
    padding:5px;  
} 

.mama{ 
    width:auto; 
    height:auto; 
    border:1px solid #000; 
    border-radius:1px; 
    padding:5px;   
}
</style>