<template>
  <div class="wrapper" ref="wrapper">
    <ul class="content">
      <li>展示1</li>
      <li>展示2</li>
      <li>展示3</li>
      <li>展示4</li>
      <li>展示5</li>
      <li>展示6</li>
      <li>展示7</li>
      <li>展示8</li>
      <li>展示9</li>
      <li>展示10</li>
      <li>展示11</li>
      <li>展示12</li>
      <li>展示13</li>
      <li>展示14</li>
      <li>展示15</li>
      <li>展示16</li>
      <li>展示17</li>
      <li>展示18</li>
      <li>展示19</li>
      <li>展示20</li>
      <li>展示21</li>
      <li>展示22</li>
      <li>展示23</li>
      <li>展示24</li>
      <li>展示25</li>
      <li>展示26</li>
      <li>展示27</li>
      <li>展示28</li>
      <li>展示29</li>
      <li>展示30</li>
      <li>展示31</li>
      <li>展示32</li>
      <li>展示33</li>
      <li>展示34</li>
      <li>展示35</li>
      <li>展示36</li>
      <li>展示37</li>
      <li>展示38</li>
      <li>展示39</li>
      <li>展示40</li>
      <li>展示41</li>
      <li>展示42</li>
      <li>展示43</li>
      <li>展示44</li>
      <li>展示45</li>
      <li>展示46</li>
      <li>展示47</li>
      <li>展示48</li>
      <li>展示49</li>
      <li>展示50</li>
    </ul>
  </div>
</template>

<script>
import BScroll from "better-scroll";

export default {
  name: 'Category',
  data() {
    return {
      scroll: null
    }
  },
  mounted() {
    this.scroll = new BScroll(this.$refs.wrapper, {
   
    })
  }
}
</script>

<style scope>
.wrapper {
  height: 150px;
  background-color: red;
  overflow: hidden;
}
</style>
