<template>
  <div>
    <ComponentFrame>
      <BadInput
        label="First name"
        labelColor="#303030"
        inputPlaceholder="Please enter your first name"
        buttonText="Confirm"
        @textChange="handleTextChange"
        @buttonClick="handleButtonClick"
      />
    </ComponentFrame>
    <ComponentFrame>
      <div>
        <Label
          text="First name"
          color="#303030"
        />
        <Input
          placeholder="Please enter your first name"
          :style="{ marginTop: '7px' }"
          @input="handleTextChange"
        />
        <Button
          text="Comfirm"
          :style="{ marginTop: '4px' }"
          @click="handleButtonClick"
        />
      </div>
    </ComponentFrame>
    <ComponentFrame>
      <InputForm
        label="First name"
        placeholder="Please enter your first name"
        @submit="handleSubmit"
      />
    </ComponentFrame>
  </div>
</template>

<script>
import BadInput from '@/components/SingleResponsibitliyPrinciple/BadInput';
import Label from '@/components/SingleResponsibitliyPrinciple/Label';
import Input from '@/components/SingleResponsibitliyPrinciple/Input';
import Button from '@/components/SingleResponsibitliyPrinciple/Button';
import InputForm from '@/components/SingleResponsibitliyPrinciple/InputForm';

export default {
  components: {
    BadInput,
    Label,
    Input,
    Button,
    InputForm,
  },
  methods: {
    handleTextChange() {
    },
    handleButtonClick() {
    },
    handleSubmit() {
    },
  },
}
</script>
