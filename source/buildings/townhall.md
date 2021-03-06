---
title: Town Hall
layout: default

---

# Town Hall

<div class="infobox box text-center">
    <img src="../../assets/images/buildings/townhall.png" alt="Town Hall's Block" />
    <hr />
    <recipe>townhall</recipe>
</div>


市政厅是你的殖民地的核心部分

注释：市政厅方块不能被合成，除非你已经放置了从[补给营地或补给船](../../source/items/supplycampandship)中获得的市政厅。
如果有必要，可以从创造模式或通过命令获得。

## 开启新殖民地

### 勘测地块

在放置市政厅之前，先确保你已经详细地勘测过要开启殖民地的地块。你的殖民地将以市政厅方块为中心，以4个区块为半径向各个方向延伸。确定这是你要开荒的地方。

### 放置你的市政厅

考虑清楚你要放置市政厅的位置以后（记住，该位置将是你的殖民地受保护范围的中心位置，这个区域将会被固定下来，不能再改变），使用[建筑工具] (../items/buildtool)来放置市政厅方块。

右击你要放置市政厅方块的地面。建筑工具GUI将展示市政厅的3D预览。你可以点击箭头按钮移动建筑到你想要的位置。

**注释:** 你要先按按GUI中的+和-按钮，确保你的小屋的地面是在你想要的水平面上。不是所有小屋的方块都会在地面上。

确定了放置位置以后（绿色勾号），市政厅方块就直接被放置下去。

### 创建你的殖民地

放置完市政厅方块以后，你需要右击，选择【创建新殖民地】。
<img src="../../assets/images/gui/th_colonycreationGUI.png" alt="Creating New Colony" />

一个新的殖民地将被创建，殖民地的范围将被确定，整个区域将受到保护。

### 区域保护

当你开启一块新的殖民地的时候，初始设置中也会添加上区域保护。保护系统包括阻止任何玩家放置或者破坏方块，或者和任何种类的方块交互，或者放置岩浆或者水，还有放置和点燃TNT也会被禁止。保护系统建立后，将被展示在屏幕信息上。

你的殖民地的保护区域（市政厅被放置后）将取决于你的设置文件，默认是4个区块为半径，以你第一次放置市政厅方块的位置为圆心。因此，你要考虑清楚你所要放置市政厅方块的位置。你的殖民地保护区域包括山地、丘陵、湖泊、海洋、洞穴，自定义世界生成的结构等，且从基岩到天空高度限制的地方都在内。

由于每一个殖民地都有区域保护，你得仔细勘察你周围的环境以确保周围没有其他殖民地，以免处于其他殖民地的保护区域内，而阻止你放置市政厅方块，或者你的殖民地在延伸上受到该方向上的限制。

**注释:** 放置市政厅方块以后，这将作为你的殖民地保护区域的【圆心】。如果你决定要让你实际的市政厅健在其他位置（在你现在设置的保护区域范围内），你可以破坏市政厅方块，然后
用建筑工具再放置一遍。移除市政厅方块后重新放置【不会】删除对你的殖民地的区域保护。删除区域保护、把市政厅挪到其他地方的唯一方法是叫有OP或者管理员权限的人用[命令](../systems/command)删除你的殖民地信息。

**注释:**你可以定义你自己殖民地的半径，在你的world/server里的config文件夹的minecolonies-common.toml里修改。

如果已有殖民地太靠近你当前的位置，你将无法放置市政厅方块。

如果你尝试在你的保护区域外放置另外的市政厅方块，你将收到一条信息如下： <br> 
<img src="../../assets/images/gui/th_secondplace.png" alt="Placing a Second Town Hall"/>

## 市政厅GUI

<i>你可以用左侧的标签页去切换条目</i>

<br>

### <strong>信息:</strong> 这是市政厅GUI的总体信息部分。

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_information.png" class="img-fluid mx-auto" alt="TH GUI Information Tab">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
          <li><strong>第一页: </strong>在这里展示出你的市民的一些统计信息。例如市民的总数以及就业情况。如果他们有工作了，你可以在这里看到他们的职业。</li>
      <br>
         <li><strong>第二页: </strong>在这里展示殖民地的整体幸福度以及在殖民地中发生的所有事件（最新的事件展示在最底部）。点击按钮切换到行为许可日志界面，在这里展示所有在殖民地中不符合设定的规则的行为（例如当规则是不允许破坏方块时有玩家尝试这样做）。 点击非法行为旁边的加号将会把它设置回合法的，当玩家再次发生该行为不再判定为非法。详见 <a href="../../source/systems/protection"> 殖民地保护系统</a>以及市政厅GUI中的权限页面。</li>
    </ul>
  </div>
</div>


<br>
<br>

### <strong>行动:</strong> 这是最重要的部分。


<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_actions.png" class="img-fluid mx-auto" alt="TH GUI Actions Tab">
  </div>
  <div class="col-sm-12 col-md">
    <p><strong>第一页: </strong>在这一页你可以看到你的殖民地的名称，市政厅的等级以及一些按钮：</p>
    <ul>
      <li><strong>Build Options 建筑选项-</strong>点击该按钮为你的市政厅下达建造、升级、移动、修复等建筑指令。想要了解更多有关建造系统的信息，请查阅<a href="../../source/workers/builder">建筑工</a>页面。</li><br>
      <li><strong>Rename Colony 重命名殖民地-</strong>更改你的殖民地的名字（默认为 你的ID+'s Colony）。</li><br>
      <li><strong>Hire Mercenaries 雇佣兵-</strong>雇佣雇佣兵来保卫殖民地，不过他们可都是些流氓，是会偷你的村民的物品的！</li>
    </ul>
    <br>  
    <p><strong>第二页: </strong>当且仅当PVP在设置文件中被开启，本页才生效。在这里你可以：</p>
    <ul>
      <li><strong>Allies 盟友-</strong>这里会显示和你结盟的殖民地。（结盟是双向的）</li>
      <br>
      <li><strong>Feuds 敌人-</strong>这里会显示和你敌对的殖民地。（敌对是双向的）</li>
    </ul>
  </div>
</div>


<br>
<br>

### <strong>权限:</strong> 在这里邀请你的好友合作开发殖民地

<p><strong>权限页面 第一页和第二页：</strong>你可以设置其他玩家在殖民地中的地位，不同的地位等级会在殖民地保护系统中有不同的特权。</p>


<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_permissions.png" class="img-fluid mx-auto" alt="TH GUI Permissions Tab">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
      <li><strong>第一页: </strong>在这里输入你想要添加权限的玩家的ID</li>
      <br>
      <li><strong>第二页: </strong>显示你已添加的玩家列表，以及他们的地位等级。你可以点击“+”或“-”来调整他们的地位。</li>
    </ul>
  </div>
</div>  



---

<p><strong>权限界面 第三页和第四页：</strong>你可以在这设置各个地位等级的权限。</p>

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_permissions2.png" class="img-fluid mx-auto" alt="TH GUI Permissions Tab Pg.2">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
      <li><strong>第三页: </strong>在这选择你要设置权限的地位等级。</li>
      <br>
      <li><strong>第四页: </strong>这里显示各项权限（给你在前一页选中的地位等级），调节 <i>开</i> 或 <i>关</i>， 以给予你想要给的权限</li> 
    </ul>
  </div>
</div>  



---


<p><strong>权限界面 第五页和第六页: </strong>在这一部分，你可以添加一个确定的方块坐标，该方块将绕过殖民地保护系统，提供给大家进行交互。只要玩家所在的地位等级包括权限“交互自由方块”，他们就可以和该方块进行交互了。</p>

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_permissions3.png" class="img-fluid mx-auto" alt="TH GUI Permissions Tab Pg.3">
  </div>
  <div class="col-sm-12 col-md">
    <ul><br>
      <li><strong>第五页: </strong>这里键入你想要让玩家自由交互的方块的位置（X,Y,Z）。</li>
      <br>
      <li><strong>第六页: </strong>这里显示能够自由交互的方块位置列表，你可以在这里移除他们。</li>
    </ul>
  </div>
</div>


<br>
<br>

### <strong>市民: </strong>这个部分将展示你的殖民地中所有市民的名字和技能，以及技能的等级


<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_citizens.png" class="img-fluid mx-auto" alt="TH GUI Citizens Tab">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
     <br>
      <li><strong>第一页: </strong>当你选定一个公民后，关于他的统计信息就会出现在这一页。你也可以在这里单独将公民召集回市政厅。</li>
      <br>
      <li><strong>第二页: </strong>这你可以看到你的公民列表，选择一个公民来查看具体的技能信息。</li>
    </ul>
  </div>
</div>


<br>
<br>

### <strong>设置: </strong>这一部分是你调整市民的工作、安排殖民地住宅的地方，以及另外一些事情

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_settings.png" class="img-fluid mx-auto" alt="TH GUI Settings Tab">
  </div>
  <div class="col-sm-12 col-md">
      <p><strong>第一页: </strong>这里有四个按钮:</p>
        <ul>
            <li><strong>Worker hiring mode 雇佣模式: </strong>点击这里可以切换自动与手动模式，自动模式下会为你自动选择最合适的工人，但你不可以在工作小屋中对任何市民进行解雇和雇佣。手动模式下，你可以在任何时候手动<i>雇佣</i>或<i>解雇</i>你想要的人选。</li>
          <br>
          <li><strong>Housing assignment mode 住宅安排模式: </strong>点击这个按钮可以切换自动模式与手动模式。若是选择了自动模式，那么公民只要一生成就会被分配一个住房（如果有可用的房屋的话）。若是选择了手动模式，那你就要自己决定公民是要住在哪一座<a href="../../source/buildings/house"> 住宅</a> 或 <a href="../../source/buildings/tavern"> 酒馆</a>里了。如果说你的殖民地足够大的话，那你就能将公民安排在最靠近其工作岗位的地方，这样就能让他快速上工了。</li>
          <br>
          <li><strong>Print help messages 输出教程信息: </strong>点击这个按钮可以决定是否在聊天栏里输出教程信息，建议初次游玩的玩家把它开启。</li>
          <br>
          <li><strong>Kids will be born 婴儿降生: </strong>点击这个按钮可以选择是否允许孩子出生在你的殖民地里。</li>p
        </ul>
		<br>
            <p><strong>第二页: </strong>这里有两个按钮:</p>
        <ul>
            <li><strong>Pick Team Color 选择队伍颜色: </strong>不管你选择了什么颜色，当你的士兵在<a href="../../source/buildings/guardtower"> 卫兵塔</a> 或 <a href="../../source/buildings/barrackstower"> 兵营塔</a>中设置为跟随模式时，他的身上都会散发相应颜色的光芒。这个选项是为PVP系统准备的，以此你可以知道在战斗的时候，哪些士兵是忠于你的。不仅如此，你的公民的名字也会变成相应的颜色。</li>
			<br>
            <li><strong>Edit Colony Flag 编织殖民地旗帜: </strong>点击这个按钮将会打开旗帜设计器，你可以在这里设计你的殖民地专有的旗帜。你的<a href="../../source/workers/guard"> 骑士</a>的盾牌上会刻画出你最终设计的图案。旗帜也会被用在其他的蓝图结构中。</li>
            <div class="col-sm-12 col-md">
			<img src="../../assets/images/gui/th_colonybannerdesigner.png" class="img-fluid mx-auto" alt="TH GUI Banner Designer">
			</div>
		</ul>
  </div>
</div>

<br>

<br>

### <strong>施工顺序: </strong>在这里你可以看到<a href="../../source/workers/builder">建筑工</a>的被安排的施工顺序。当且仅当最上面的任务顺利完成了，建筑工才会进行下一个任务

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_workorders.png" class="img-fluid mx-auto" alt="TH GUI Work Orders Tab">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
      <li><strong>第一页: </strong>仅显示了标题的空白页码，留作备用。</li>
      <br>
      <li><strong>第二页: </strong>这里是殖民地所有的施工任务的列表（包括装饰，你的自定义蓝图以及各种小屋），你的工人将会按照从上往下的顺序进行建造，你可以通过拖拽来改变建造的先后。你也可以对施工任务进行撤销。当你撤销正在进行的施工任务后，你的工人将会中止建筑，若是你再次安排该任务，那么工人就会在旧址继续进行建造。</li>
    </ul>
  </div>
</div>

<br>
<br>

### <strong>幸福: </strong>这一部分显示你的殖民地的总体幸福度，以此你可以看到哪些地方需要多加关注以提升幸福水平

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/th_happiness.png" class="img-fluid mx-auto" alt="TH GUI Work Orders Tab">
  </div>
  <div class="col-sm-12 col-md">
    <ul>
      <br>
      <li><strong>第一页: </strong>幸福度的指标。你可以在这里查看哪些东西会影响公民的幸福度。关于颜色（由好到坏）：绿色（积极）、蓝色（素净）、黄色（沉闷）、红色（消极）。除此之外，还有黑色，显示的时候代表某事出现问题了。</li>
      <br>
      <li><strong>第二页: </strong>空白，留作备用</li>
    </ul>
  </div>
</div>  


<br>
